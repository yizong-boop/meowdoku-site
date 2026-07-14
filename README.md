# Meowdoku HTML 文档站

这是一个可直接发布到 Netlify 的静态站点。

## 发布

将 `meowdoku_site` 整个文件夹作为 Netlify 的发布目录，或直接拖拽该文件夹上传。入口文件是 `index.html`，不需要构建命令。

## 内容

- 亮色主题、响应式布局、左侧章节导航和全文搜索；
- 主玩法棋盘交互示例；
- 普通关、Daily、连胜、道具、广告、配置、埋点和验收清单；
- 当前 APK 资源包中的猫咪、道具、生命、胜利、连胜和棋盘素材精选预览；
- Daily 页面截图位置已预留，当前不嵌入不对应页面的运行截图；
- BGM / SFX 资源索引；
- `resources.html` 全量资源考察站：528 条资源记录，含 274 张图片、82 条可试听 OGG、Spine/Godot 动效组成文件、多语言、题库 JSON、字体和场景资源；
- `resource-catalog.json` 可供研发或脚本二次消费的完整清单。

音频原始形态是 Godot 的 `.oggvorbisstr` 导入流格式，已通过 GDRE 恢复成浏览器可播放的 `.ogg`。APK 中没有发现 GIF、WebM 或 MP4；动效主要是 Spine 4.2.43 的 `.skel + .atlas + .png` 和 Godot `.tres/.res`。

如需本地预览动态资源站，可在 `meowdoku_site` 目录启动任意静态 HTTP 服务后打开 `resources.html`；直接双击 HTML 可能会被浏览器的本地文件安全策略拦截 JSON 加载。
