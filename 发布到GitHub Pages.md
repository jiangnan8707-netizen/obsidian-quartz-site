# 发布到 GitHub Pages

这个文件夹已经是一个 Quartz 静态笔记站项目。

## 第一次发布

1. 在 GitHub 新建一个公开仓库，建议仓库名使用 `obsidian-quartz-site`。
2. 在这个文件夹里连接你的 GitHub 仓库并推送：

```powershell
git remote add origin https://github.com/你的用户名/obsidian-quartz-site.git
git branch -M main
git push -u origin main
```

3. 打开 GitHub 仓库的 `Settings` -> `Pages`。
4. 在 `Build and deployment` 里把 `Source` 设为 `GitHub Actions`。
5. 等待 Actions 运行完成，网站地址会显示在 Pages 页面里。

## 后续更新

把新的 Markdown 笔记放进 `content` 文件夹，提交并推送到 GitHub 后，网站会自动更新。

```powershell
git add content
git commit -m "Update notes"
git push
```

## 注意

- `content/private`、`content/templates` 和 `.obsidian` 不会发布。
- 静态网站没有登录限制，发布后的内容拿到链接就能看。
- 当前站点标题在 `quartz.config.ts` 里是 `我的 Obsidian 笔记`，可以按需要改名。
