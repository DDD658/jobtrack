# 投递收件箱 · JobTrack

本项目是纯前端静态网站，可通过 GitHub Pages 发布。无需构建步骤，也不需要提交求职数据。

## 本地预览

直接用现代浏览器打开 `index.html`。OCR 与 PDF 文字解析首次使用时会从 CDN 加载浏览器端开源库和语言包，因此需要联网；识别内容在浏览器本地处理。

## 发布到 GitHub Pages

1. 在 GitHub 创建一个**公开**仓库（例如 `jobtrack`）。
2. 将本目录中的文件上传到仓库根目录：`index.html`、`README.md`、`.nojekyll`。
3. 打开仓库 **Settings → Pages**。
4. 在 **Build and deployment** 选择 **Deploy from a branch**。
5. Branch 选择 `main`，目录选择 `/(root)`，保存。
6. 等待 GitHub Pages 部署完成，页面会显示公开网址，通常形如 `https://你的用户名.github.io/jobtrack/`。

若仓库名为 `你的用户名.github.io`，网址通常是 `https://你的用户名.github.io/`。

## 数据与隐私

- 所有投递、简历和微日志保存在访问者自己的浏览器本地，不会在用户之间同步。
- 不要把个人求职记录、简历文件或备份 JSON 提交到 GitHub 仓库。
- 公开仓库中的网页任何人都能查看和使用；每个人的数据仍相互隔离在各自浏览器中。
- OCR / PDF 依赖首次从 CDN 加载；AI 建议使用本地规则生成。复杂分析可复制 Prompt 到用户自行选择的工具。
- 清除浏览器数据可能导致记录丢失，请定期在设置页导出备份。

## 当前结构

```text
index.html   网站主体（样式和脚本均内嵌）
README.md    本说明与 GitHub Pages 发布步骤
.nojekyll    告知 Pages 按静态文件发布
```
