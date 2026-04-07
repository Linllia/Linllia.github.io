---
layout: post              # 使用 post 布局
title: "Tmux note"
date: 2026-04-07 20:23:00 +08:00
categories: [Tech]  # 分类（会在博客页面按分类分组）
tags: [Tools, Note]      # 标签
code: true               # 启用代码高亮
math: false              # 是否启用数学公式
mermaid: false           # 是否启用 Mermaid 图表
excerpt: 学习使用Tmux
---


## tmux三层结构
```
session（会话）
 ├─ window（窗口）
 │   ├─ pane（面板/分屏）
 │   └─ pane
 └─ window
```

## session
session是一个工作空间
创建
```
tmux new -s dev
```
查看目前有的session
```
tmux ls
```
使用某个session
```
tmux attach -t dev
```
离开tmux但是仍继续运行（这个叫做detach
```
ctrl+b d
```

## window
window是窗口
就是tmux下方数字代表的
创建新窗口
```
ctrl+b c
```
切换下一个窗口
```
ctrl+b n
```
切换上一个窗口
```
ctrl+b p
```
直接切换到对应数字的窗口
```
ctrl+b 0/1/2
```
关闭窗口
```
ctrl+b &
```
如果只有一个pane的话直接exit

## pane
pane是每个窗口里的小格
左右分屏
```
ctrl+b %
```
上下分屏
```
ctrl+b “
```
切换pane
```
ctrl+b ⬆️⬇️⬅️➡️
```
关闭pane
```
exit
```




