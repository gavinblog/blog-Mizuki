---
title: astro博客快速开始
description: 简单介绍astro博客的使用方法，快速开始搭建一个自己的博客
published: 2026-01-11
author: geekswg
category: astro
tags: [astro,demo]

# 封面
image: /assets/imgs/logo.webp
---

## 准备

1. 安装 [Node.js](https://nodejs.org/) 和 [npm](https://www.npmjs.com/)
2. 安装 [Astro CLI](https://astro.build/install/auto)

```bash
npm install -g astro
```

## 创建项目

1. 使用astro cli创建项目
```bash
astro create blog-astro
```

2. fork主题创建自己的博客,(推荐使用)
如 访问[mizuki主题仓库](https://github.com/matsuzaka-yuki/mizuki),点击`fork`按钮，fork到自己的仓库中，然后克隆到本地。

```bash
git clone https://github.com/matsuzaka-yuki/mizuki.git
```
:::note
推荐fork主题安装因为可以方便的更新主题，如果使用astro cli创建的项目，需要手动更新主题。
:::

## 运行项目

1. 安装依赖
```bash
pnpm install
```
2. 运行
```bash
pnpm run dev
```
如果控制台出现
```
 astro  v5.16.4 ready in 4769 ms

┃ Local    http://localhost:4321/
┃ Network  use --host to expose

11:08:06 watching for file changes...

```
3. 打开浏览器访问 `http://localhost:4321`

## 常用语法

### Admonitions

Following types of admonitions are supported: `note` `tip` `important` `warning` `caution`

:::note
Highlights information that users should take into account, even when skimming.
:::

:::tip
Optional information to help a user be more successful.
:::

:::important
Crucial information necessary for users to succeed.
:::

:::warning
Critical content demanding immediate user attention due to potential risks.
:::

:::caution
Negative potential consequences of an action.
:::

```
## Admonitions

Following types of admonitions are supported: `note` `tip` `important` `warning` `caution`

:::note
Highlights information that users should take into account, even when skimming.
:::

:::tip
Optional information to help a user be more successful.
:::

:::important
Crucial information necessary for users to succeed.
:::

:::warning
Critical content demanding immediate user attention due to potential risks.
:::

:::caution
Negative potential consequences of an action.
:::
```