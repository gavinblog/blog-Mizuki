---
title: js的魔法特效
description: "记录一些神奇且实用的JavaScript特效，源码来自互联网，部分经过修改和优化。"
published: 2026-01-19T18:51:00+08:00

keywords: ["js","javascript","geekswg","毕少侠"]
tags: ["js","javascript"]
category: "dev"
---

## 游动的小鱼

<a href="javascript:window.scrollTo(0, document.body.scrollHeight);" >查看效果 </a>

flyfish.js脚本源码： [js/my/flyfish.js](/js/my/flyfish.js)

## 动态彩虹带背景

> 使用方法：直接在html中引入下面的js代码即可。
```js
<script src="/js/my/ribbons.js"></script>
```
<a href="javascript:loadJS('/js/my/ribbons.js')">查看效果</a>

[ribbons.js脚本源码](/js/my/ribbons.js)

## canvas数字时钟

效果见主页或者侧边栏的数字时钟。

使用方法：将下面的html代码放到你想显示数字时钟的位置，并引入canvasTime.js脚本即可,可以通过colckColor参数指定时钟的颜色，如果没有指定，则七种颜色随机生成。

```html
<!-- 数字时钟 -->
<div class="aside-custom" >
  <canvas style="width:100%;" id="canvasTime" >当前浏览器不支持canvas，请更换浏览器后再试</canvas>
</div>
<script src="/js/canvasTime.js?colckColor=red" ></script>
```
[canvasTime.js脚本源码](/js/canvasTime.js)

## 飞舞雪花

<a href="javascript:startSnow()">开始下雪</a>
<a href="javascript:stopSnow()">停止下雪</a>

> 查看源码 [js/my/flysnow.js](/js/flysnow.js)

<script>
  function startSnow(){
    if (!window.snowfall) {
      loadJS('/js/my/flysnow.js?snowColor=f00');
    } else if (!window.snowfall.isRunning) {
      window.snowfall.toggle();
    }
  }
  function stopSnow(){
    if (window.snowfall) {
      window.snowfall.destroy();
      window.snowfall = null;
    }
  }
  function loadJS(src){
    var script = document.createElement('script');
    script.src = src;
    document.head.appendChild(script);
  }
</script>

<!--
> [!NOTE]
> 突出显示用户应考虑的信息，即使只是浏览也应考虑。

> [!TIP]
> 可选信息，可帮助用户取得更大的成功。

> [!IMPORTANT]
> 用户成功所需的关键信息。

> [!WARNING]
> 由于存在潜在风险，需要用户立即关注的关键内容。

> [!CAUTION]
> 操作的潜在负面后果。
这里使用MD语法编写你的文章
 -->