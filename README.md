# xxwlive.github.io

夏祥伟的个人博客「遥远612星球」，基于 [Fuwari](https://github.com/saicaca/fuwari)（Astro）搭建，部署在 GitHub Pages。

## 写文章

在 `src/content/posts/` 下新建 Markdown 文件，文件头示例：

```yaml
---
title: 文章标题
published: 2026-09-22
description: 一句话简介
tags: [标签]
category: 分类
draft: false
---
```

也可以运行 `pnpm new-post 文件名` 自动生成。推送到 `main` 后，GitHub Actions 会自动构建并发布。

## 本地预览

```sh
pnpm install
pnpm dev       # 开发模式，http://localhost:4321
pnpm build     # 构建到 dist/
```

## 常改的地方

- 站点标题、头像、简介、链接、横幅：`src/config.ts`
- 关于页：`src/content/spec/about.md`
- 图片：`src/assets/images/`
