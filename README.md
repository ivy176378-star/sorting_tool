# 我的排序器 (interest-sorter)

单文件、零依赖的静态页面：兴趣排序、分类管理、转盘抽签。所有数据保存在浏览器 `localStorage`，不上传服务器。

## 使用方式

- 在线访问：<https://ivy176378-star.github.io/sorting_tool/>
- 本地使用：直接双击 `index.html`，或在目录下执行 `python3 -m http.server` 后访问 `http://localhost:8000`。

## 说明

- `index.html` 为完整单文件页面（内联 CSS / JavaScript、Canvas 转盘、Web Audio 音效），无需构建、无需安装依赖。
- 本页由 WorkBuddy 资料库 Page 迁移而来，已移除宿主注入脚本 `/page/page_comm/inject.js` 与编辑器锚点属性，可脱离资料库独立运行。
- 浏览器数据按域名隔离：线上版本、本地版本、资料库版本之间的排序与抽签历史互不相通。
- 仓库中的 `.github/workflows/pages.yml` 用于生成页面并部署 GitHub Pages；页面生成后会提交回仓库，后续构建不再依赖外部资源。
