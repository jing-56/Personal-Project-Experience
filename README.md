# 个人作品站模板

这是一个可以直接放到 GitHub Pages 的静态个人作品站。你只需要替换 `index.html` 里的名字、项目介绍、联系方式，以及 `assets/` 里的图片。

## 本地预览

直接双击打开 `index.html` 即可预览。

如果想用本地服务器预览，也可以在这个目录运行：

```bash
python -m http.server 8000
```

然后访问 `http://localhost:8000`。

## 部署到 GitHub Pages

1. 新建或打开 GitHub 仓库，比如 `Personal-Project-Experience`。
2. 把本目录下的所有文件推送到仓库根目录。
3. 在 GitHub 仓库设置里打开 `Settings -> Pages`。
4. `Build and deployment` 选择 `Deploy from a branch`。
5. 分支选择 `main`，目录选择 `/root`，保存。
6. 等待 GitHub Pages 构建完成后访问生成的站点链接。

## 建议替换项

- 姓名：王嘉璐。
- 邮箱：`962447890@qq.com`。
- GitHub：`https://github.com/jing-56`。
- 项目卡片里的标题、简介和链接。
- `assets/project-*.png` 和 `assets/photo-*.png`：替换成项目截图和摄影作品。

## Hugo / Jekyll 迁移说明

这个版本是无构建静态站，最适合快速上线。后续如果要迁到 Hugo 或 Jekyll，可以把当前页面拆成：

- `layouts/index.html` 或 `_layouts/default.html`
- `content/projects/*.md` 或 `_posts/*.md`
- `static/assets/` 或 `assets/`

现有的 HTML 和 CSS 可以继续复用。
