---
title: "MEGASync 多实例管理器"
date: 2025-09-16
draft: false
description: "一个与发行版无关的脚本，用于为不同的 MEGA 帐户管理多个 MEGASync 实例。"
tags: ["megasync", "linux", "bash", "脚本", "个人项目"]
---

一个与发行版无关的脚本，用于为不同的 MEGA 帐户管理多个 MEGASync 实例。

![Megasync 管理器](featured.png)

## 功能
- 适用于 Debian、Ubuntu、Fedora 和 Arch Linux
- 使用 Zenity 提供图形界面
- 独立实例，拥有各自的配置目录
- 动态添加实例
- 实例持久化存储

{{< github repo="geraldohomero/megasync-multiple-instances" >}}

## 安装

运行以下命令安装：

```bash
wget -O - https://raw.githubusercontent.com/geraldohomero/megasync-multiple-instances/refs/heads/main/megasync-manager.sh | bash -s install
```

然后使用：

```bash
mega
```

该脚本会检测你的发行版并安装依赖（`megasync`、`zenity`）。

## 使用

- 运行 `mega` 打开管理器。
- 选择要启动的实例或添加新实例。
- 配置实例自动启动。
