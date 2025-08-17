# 基于  hugo 生产 github page

1. Hugo 是用 Go 实现的博客工具，采用 Markdown 进行文章编辑，自动生成静态站点文件，支持丰富的主题配置，也可以通过
js 嵌入像是评论系统等插件，高度定制化。
2. 当前主题使用[hugo-brewm](https://github.com/foxihd/hugo-brewm)

## 文档

- [Hugo + Github Pages 搭建个人博客](https://jianzhnie.github.io/post/hugo_site/)
- [Hugo](https://gohugo.io/)
- [Themes](https://themes.gohugo.io/)

## Deepseek 生成文档

```bash
# 1. 创建 Hugo 项目
hugo new site my-hugo-site
cd my-hugo-site

# 2. 添加主题（以 ananke 为例）
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
echo "theme = 'ananke'" >> config.toml

# 3. 创建测试文章
hugo new post/first-post.md

# 4. 修改 config.toml 关键配置
echo 'baseURL = "https://<你的用户名>.github.io/<仓库名>/"' >> config.toml
echo 'publishDir = "docs"' >> config.toml  # 指定输出目录

# 5. 生成静态文件
hugo

# 6. 推送到 GitHub
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/<你的用户名>/<仓库名>.git
git push -u origin main

# 7. 启用 GitHub Pages
# 仓库 Settings → Pages → Branch: main → Folder: /docs
```