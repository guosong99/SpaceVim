---
title: "SpaceVim edit 模块"
description: "这一模块为 SpaceVim 提供了更好的文本编辑体验，提供更多种文本对象。"
lang: cn
---

# [可用模块](../) >> edit

<!-- vim-markdown-toc GFM -->

- [模块简介](#模块简介)
- [功能特性](#功能特性)
- [模块选项](#模块选项)
- [快捷键](#快捷键)

<!-- vim-markdown-toc -->

## 模块简介

该模块提升了 SpaceVim 的文本编辑体验，提供更多种文本对象。

## 功能特性

- 修改围绕当前光标的符号
- 重复编辑
- 多光标支持
- 对齐文档内容
- 设置文档段落对齐方式
- 高亮行为符号
- 自动载入 editorconfig 配置，需要 `+python` 或者 `+python3` 支持
- 默认已启用

## 模块选项

- `textobj`: specified a list of text opjects to be enabled, the avaliable list is: `indent`, `line`, `entire`

## 快捷键

| 快捷键             | 功能描述               |
| ------------------ | ---------------------- |
| `SPC x a {分隔符}` | 基于分隔符进行文本对齐 |

**默认的分隔符：**

- `=`: 对齐 `===`, `==`, `!=`, `>=` 等
- `&`: 对齐 `&`
- `¦`: 对齐 `¦`
- `|`: 对齐 `|`
- `;`: 对齐 `;`
- `:`: 对齐 `:`
- `,`: 对齐 `,`
- `.`: 对齐 `.`
- `[`: 对齐 `[`
- `(`: 对齐 `(`
- `{`: 对齐 `{`
- `]`: 对齐 `]`
- `}`: 对齐 `}`
- `)`: 对齐 `)`
- `[SPC]`: 对齐 `[SPC]`
- `o`: 对齐 `+ - * / % ^` 等

| 快捷键       | 功能描述                             |
| ------------ | ------------------------------------ |
| `SPC x j c`  | 居中对齐当前段落                     |
| `SPC x j f`  | set the justification to full (TODO) |
| `SPC x j l`  | 左对齐当前段落                       |
| `SPC x j n`  | set the justification to none (TODO) |
| `SPC x j r`  | 右对齐当前段落                       |
