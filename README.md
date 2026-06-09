# 我的 Obsidian 静态笔记站

这是用 Quartz 生成的 Obsidian 静态笔记站。公开内容放在 `content` 文件夹里，推送到 GitHub 后会通过 GitHub Pages 自动发布。

## 本地预览

```powershell
npm install
npx quartz build --serve
```

打开本地预览地址后，可以检查首页、搜索、目录、反向链接和图谱是否正常。

## 构建

```powershell
npx quartz build
```

构建结果会生成到 `public` 文件夹。

## 发布

第一次发布请参考 [发布到GitHub Pages.md](发布到GitHub%20Pages.md)。
