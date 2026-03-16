# 文字转语音工具 (Text-to-Speech Pro) - PWA

这是一个使用 Web Speech API 的文字转语音工具，现在已转换为 Progressive Web App (PWA)。

## 功能特性

- 支持多种语音选择
- 可调节语速、音调和音量
- 实时文本高亮显示
- 支持音频导出 (WAV/MP3)
- 离线可用 (PWA)

## PWA 配置

项目已配置为 PWA，包括：

- Web App Manifest (`manifest.json`)
- Service Worker (`sw.js`) 用于缓存和离线支持
- 图标目录 (`icons/`)

## 部署

1. 确保所有文件都在同一目录
2. 部署到支持 HTTPS 的服务器 (PWA 需要 HTTPS)
3. 用户可以从浏览器安装应用

## 本地测试

使用本地服务器测试 PWA 功能：

```bash
# 使用 Python
python -m http.server 8000

# 或使用 Node.js
npx serve .
```

然后访问 `http://localhost:8000` 并检查应用是否可以安装。

## 文件结构

```
/
├── index.html          # 主应用界面
├── simple-tts.html     # 简单示例页面
├── manifest.json       # PWA 清单
├── sw.js              # Service Worker
└── icons/             # 应用图标
    ├── icon-192.png
    └── icon-512.png
```