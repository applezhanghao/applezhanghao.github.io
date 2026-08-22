# AppDownload Guide — Jekyll 版

这是可由 GitHub Pages 直接构建的 Jekyll 项目。上传此目录的全部内容到 `applezhanghao.github.io` 仓库根目录后，GitHub Pages 会自动检测 `_config.yml` 并构建网站。本项目不附带 Gemfile，因此会使用 GitHub Pages 自带的 Jekyll 构建环境。

## 更新首页内容

首页的设备、入口卡、商品展示与 FAQ 位于 `_data/site.yml`。修改该文件后提交即可更新首页对应模块。

## 新增文章

复制 `templates/article-template.md` 到 `_articles/`，修改标题、日期、摘要与正文。新文章会自动生成 `/articles/文件名/` 路径并写入 `sitemap.xml`。

## 新增普通说明页面

可复制 `download-shadowrocket.md`，调整 front matter 中的标题、简介、卡片、步骤、FAQ 与 related 链接。保存到项目根目录后，Jekyll 会生成同名路径。

## 发布设置

仓库中不要放 `.nojekyll`，因为本项目需要 GitHub Pages 运行 Jekyll。进入 **Settings → Pages**，选择默认分支的 `/(root)`，GitHub 会自动构建。
