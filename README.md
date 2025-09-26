# 全景导航站点

- 打开 `index.html` 即可浏览主页。
- 主页含 10 个图片入口；悬停时图片会等比例略微放大。
- 每个分页面包含：文字输入区、全景图片空间（21:9 容器）、视频空间（16:9 容器）。

## 替换图片与媒体
- 首页入口图：编辑 `index.html` 内 `<img src="...">` 链接。
- 分页面全景图：在分页面中找到 `<div class="panorama">`，可将其替换为 `<img src="你的全景图">`。
- 分页面视频：在 `<video>` 标签上设置 `src`（可指向本地 `assets` 下文件或网络地址）。

## 本地预览
可使用任意静态服务器（例如 Python）：

```bash
cd /workspace
python3 -m http.server 8000
# 浏览器访问 http://localhost:8000
```

