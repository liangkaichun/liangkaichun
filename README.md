# 工具箱

一个精心整理的静态网页工具与小游戏合集，无需安装，即开即用。 

## 功能概览

### 媒体娱乐

| 工具 | 说明 |
|------|------|
| Simple Radio | 在线收音机 |
| RadioFM | FM 电台播放器 |
| TVPlayer | 在线电视播放 |
| M3U播放器 | M3U 音频播放器 |
| 手持弹幕LED生成器 | 生成手持弹幕效果 | 

### 益智游戏

| 游戏 | 说明 |
|------|------|
| 五子棋 | 经典棋盘对弈 |
| 9路围棋 | 经典棋盘对弈 |
| 数独 | 逻辑填数挑战 |
| 24点挑战 | 算术益智游戏 |
| 24点求解器 | 自动计算解法 |
| 俄罗斯方块 | 经典方块游戏 |
| 扫雷 | 经典扫雷游戏 |
| 舒尔特方格 | 注意力训练 |

### 效率工具

| 工具 | 说明 |
|------|------|
| 番茄钟 | 专注时间管理 |
| Roam Capture | 快速笔记捕捉 |

### 学习教育

| 工具 | 说明 |
|------|------|
| 中考单词背诵 | 英语词汇记忆 |

## 特性

- **纯静态**：所有工具均为单页 HTML 文件，无需后端服务
- **即开即用**：直接在浏览器中打开即可使用
- **响应式设计**：适配桌面端和移动端
- **零依赖**：无需安装任何依赖或框架
- **PWA 支持**：可添加到主屏幕作为独立应用使用

## 快速开始

### 本地预览

1. 克隆仓库
   ```bash
   git clone https://github.com/your-username/toolbox.git
   cd toolbox
   ```

2. 启动本地服务器（任选其一）
   ```bash
   # 使用 Python
   python -m http.server 8080

   # 使用 Node.js
   npx serve .

   # 使用 PHP
   php -S localhost:8080
   ```

3. 打开浏览器访问 `http://localhost:8080`

### 部署

本项目为纯静态网站，可部署到任意静态托管平台：

- GitHub Pages
- Vercel
- Netlify
- Cloudflare Pages

## 目录结构

```
.
├── index.html          # 主页
├── manifest.json       # PWA 配置
├── logo.svg           # Logo 图标
├── service-worker.js  # Service Worker
├── RadioFM.html       # FM 电台
├── TVPlayer.html      # 电视播放器
├── m3u.html           # 在线收音机
├── m3u-player.html    # M3U 播放器
├── led.html           # LED 弹幕生成器
├── Gomoku.html        # 五子棋
├── go9.html           # 9路围棋
├── sudoku.html        # 数独
├── Game-24.html       # 24点挑战
├── 24.html            # 24点求解器
├── tetris.html        # 俄罗斯方块
├── mine.html          # 扫雷
├── schulte.html       # 舒尔特方格
├── Pomodoro.html      # 番茄钟
├── roam.html          # Roam Capture
├── lingo.html         # 单词背诵
└── ...
```

## 添加新工具

在 `index.html` 中找到 `TOOLS` 数组，按照以下格式添加新工具：

```javascript
{ name: "工具名称", desc: "工具描述", icon: "emoji图标", href: "./链接.html", category: "分类" }
```

分类可选值：`media`（媒体娱乐）、`game`（益智游戏）、`tool`（效率工具）、`learn`（学习教育）

## 技术栈

- HTML5 / CSS3 / JavaScript
- 无外部框架依赖
- PWA (Progressive Web App)

## 开源协议

MIT License

## 贡献

欢迎提交 Issue 和 Pull Request！
