---
title: Mono-Web
description: 关于Mono-Web的由来
---

# 什么是Monoweb

我希望能找到一种舒适的记录方式，理想的状态是：在本地随手记录、整理、归纳，无感自动同步到一个静态网站，对外发布和展示。

这些内容并不局限于博客，它可能包括：

- 零散的博客
- 分章节的电子文档
- 项目介绍
- 个人介绍
- 实验记录
- 组会Slides
- ……

## 本地记录：以 Obsidian 为中心

在本地，我主要使用 Obsidian 作为核心笔记软件，虽然 Obsidian 的社区非常强大，但它更像是一间“毛坯房”，需要通过插件来搭建出想要的工作流。

## 静态站点：从 Nolebase 到结构化发布

静态站点生成器（SSG）有很多选择，但随着 LLM CLI 的发展，以及日常研究中对大模型的依赖越来越深，我开始意识到：

> 记录不仅仅是展示，它还应该能参与并加速研究过程

## 为什么是 Monoweb

因此我需要的框架是：

- 在本地延续 Obsidian 的写作习惯
- 在发布端拥有清晰的结构划分
- 同时方便接入 LLM，辅助整理与研究

但我没有足够精力维护一个完整的主题项目，因此我找到了两个能完美符合我需求的主题：

- **Wiki / 文档部分**：基于 [Fumadocs](https://www.fumadocs.dev/)
- **Blog 部分**：基于 [Mizuki](https://github.com/matsuzaka-yuki/Mizuki)

## 目录组织

当前我的项目目录如下：

```bash
.
├── blog
│   └── blog code (Mizuki)
├── wiki
│   └── wiki code (Fumadocs)
└── content
    ├── blog-content (blog仓库)
    └── wiki-content (wiki仓库)
```

共计 4 个 GitHub 仓库来维护

在本地 `blog-content` 和 `wiki-content` 分别是单独的 obsidian vault