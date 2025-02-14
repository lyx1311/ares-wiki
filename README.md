# ARES Wiki

欢迎使用 ARES 社团 Wiki！请按照以下步骤添加新的文档并更新项目结构。

## 目录结构

在主分支（main）中：

- `docs/` 目录存放所有 Markdown 文档，子目录结构需要与 `mkdocs.yml` 中的导航结构对应。
- `mkdocs.yml` 用于配置网站的结构和导航。默认情况下，文件路径从 `docs/` 目录开始。

gh-pages 分支由 GitHub Actions 在用户提交更改后自动更新。

## 添加新的 Markdown 文档

1. 在 `docs/` 目录下创建新的子目录和 Markdown 文件，确保子目录结构与 `mkdocs.yml` 中的导航结构一致。

2. 在 `mkdocs.yml` 文件中的 `nav` 部分添加该文件的链接。例如：
   
   ```yaml
   nav:
     - 首页: index.md
     - 新目录：
         - new_folder/new_file.md
   ```

3. 提交更改后，推送到远程仓库，确保其他团队成员拉取更新。