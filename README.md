# CMPT LAB website

Adapted from https://github.com/chitra-lab/chitra-lab.github.io
at commit b99b300f93cbea0135f21e4963f721d78bccda84.
The upstream MIT notice is in LICENSE.

## 部署到现有 GitHub Pages

1. 解压，把源码文件和文件夹放到现有网站仓库根目录。务必上传
   `_config.yml`、`_data`、`_includes`、`_layouts` 和 `_posts`。
2. 在同一次提交中删除旧的根目录 `index.html`，新版首页是 `index.md`。
   若曾上传静态多页版，删除旧的 research、publications、join 目录里的
   `index.html`，以及旧的 `people/index.html` 和 `style.css`。
   如果仓库有 `.nojekyll`，也要移除以启用 Jekyll。
3. 保留 `CNAME` 的内容为 `cmptlab.com`。Pages 发布来源选
   Deploy from a branch，分支选 main，目录选 /(root)。
4. 提交后查看 Actions 中的 Pages 部署记录，再打开首页、/news/ 和 /join/。

## 更新 News

在 `_posts` 里复制一篇 Markdown，改成 `YYYY-MM-DD-short-title.md`，
并修改标题、正文和链接。首页自动显示最新三条，News 归档每页五条。

## 本地预览

安装 Ruby 和 Bundler 后运行 `bundle install`，再运行
`bundle exec jekyll serve`。打开 http://localhost:4000/。

## 图片来源

首页校门照片来自 Wikimedia Commons，作者 Nishino Asuka，许可 CC BY-SA 4.0。
https://commons.wikimedia.org/wiki/File:Northwestern_Polytechnical_University_Chang%27an_Campus_Gate.jpg
照片原文件随站点提供，网页通过 CSS 调整显示尺寸。
