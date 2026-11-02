# 我的第一个仓库 · 纯静态版

> 一个用来学习 Git 与 GitHub 的最小项目，不需要 Node.js、不需要 npm，一个 `index.html` 就能跑起来。

## 项目简介

这是软件工程课程第 10 周「Git & GitHub 入门」的配套练习仓库。目标是让同学在机房电脑（可能装不了 Node）也能完成最基本的版本控制流程：

- 克隆仓库 → 修改文件 → 提交 → 推送
- 开启 GitHub Pages，让作业直接在线上可访问

## 文件结构

```
plain/
├── index.html    # 全部代码都在这里，HTML + CSS + 少量 JS
└── README.md
```

就这么多。没有打包步骤，没有依赖。

## 本地预览

任选一种方式：

```bash
# 方式 1：直接双击 index.html 在浏览器打开
# 方式 2：Python 内置静态服务器（推荐，避免某些浏览器对本地文件的限制）
python -m http.server 8080
# 然后访问 http://localhost:8080
```

## 部署到 GitHub Pages

1. 把仓库推到 GitHub（`main` 分支）
2. 进入仓库 **Settings → Pages**
3. Source 选 `Deploy from a branch`，Branch 选 `main`，文件夹选 `/(root)`
4. 保存，1~2 分钟后就能通过 `https://ylyl2711.github.io/plain/` 访问

## 练手清单

改一改这些地方，然后走一遍 `git add → git commit → git push`：

- 「自我介绍」里的姓名、班级、学号
- 「课程清单」里的状态标签（把「未开始」改成「已完成」）
- 点一下「给我点赞」按钮，体验页面交互

## 常用 Git 命令速查

```bash
git status              # 看当前改了什么
git add .               # 把所有改动加入暂存区
git commit -m "做了xxx"  # 提交到本地仓库
git push origin main    # 推送到 GitHub
```
