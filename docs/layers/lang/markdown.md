---
title: "SpaceVim lang#markdown layer"
description: "Edit markdown within vim, autopreview markdown in the default browser, with this layer you can also format markdown file."
---

# [Available Layers](../../) >> lang#markdown

<!-- vim-markdown-toc GFM -->

- [Description](#description)
- [Install](#install)
- [formatting](#formatting)
  - [options](#options)
- [Key bindings](#key-bindings)

<!-- vim-markdown-toc -->

## Description

This layer is for editing markdown file.

## Install

To use this configuration layer, update custom configuration file with:

```toml
[[layers]]
  name = "lang#markdown"
```

## formatting

SpaceVim use remark to formatting markdown file, so you need to install this program. You can install it via npm:

```sh
npm -g install remark
npm -g install remark-cli
npm -g install remark-stringify
```

### options

**listItemIndent**

How to indent the content from list items (`tab`, `mixed` or 1 , default: 1).

- `'tab'`: use tab stops (4 spaces)
- `'1'`: use one space
- `'mixed'`: use `1` for tight and `tab` for loose list items

**enableWcwidth**

Enable/Disable wcwidth for detecting the length of a table cell, default is 0. To enable this option, you need to install [wcwidth](https://www.npmjs.com/package/wcwidth)

**listItemChar**

Bullet marker to use for list items (`'-'`, `'*'`, or `'+'`, default: `'-'`).

## Key bindings

| Key bindings | mode   | Descriptions               |
| ------------ | ------ | -------------------------- |
| `SPC b f`    | Normal | Format current buffer      |
| `SPC l ft`   | Normal | Format table under cursor  |
| `SPC l p`    | Normal | Real-time markdown preview |
