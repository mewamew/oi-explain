# oi-explain 项目说明

## 项目目的

这是一个用 HTML 静态页面记录 OI（算法竞赛）题解的项目，部署在 GitHub Pages 上。

**在线地址：** https://mewamew.github.io/oi-explain/

## 项目结构

- `index.html` — 题解目录页，列出所有题解入口
- `T{题目ID}_{比赛}_{题目名}_题解.html` — 单题题解页，包含题面、题解思路、完整代码三个 Tab

## 页面规范

每道题解 HTML 包含三个面板（通过顶部 Tab 切换）：
1. **题面** — 题目背景、描述、输入输出格式、样例、数据范围
2. **题解** — 算法分析、解题思路（按步骤拆解）
3. **完整代码** — 模块化代码 + 完整提交版本（折叠展示）

## 前端风格

采用 Mewa **Armored Systems** 设计语言：
- 浅色底盘（`#f2f3ef`）+ 深海军蓝装甲（`#142138`）
- Header 和 Nav 使用深海军蓝背景，白色文字
- 代码块使用深色海军背景（`#131c2e`）
- 字体：JetBrains Mono（代码/标签）+ 系统 sans-serif（正文）
- 间距紧凑，工程感强，适合长时间阅读

## 添加新题解流程

1. 创建新的题解 HTML 文件（参考现有题解的 HTML 结构）
2. 在 `index.html` 的 `<!-- SOLUTION_LIST_START -->` 和 `<!-- SOLUTION_LIST_END -->` 之间添加对应的 `<li>` 条目
3. 提交到 GitHub，GitHub Pages 自动部署
