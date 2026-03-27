# 人格图谱 · 深度测评 PWA

七大心理学框架 · 58道题 · 深度人格测评

## 文件结构

```
persona-app/
├── index.html      ← 主应用（完全自包含）
├── manifest.json   ← PWA 应用配置
├── sw.js           ← Service Worker（离线支持）
├── icon-192.svg    ← 应用图标 192px
├── icon-512.svg    ← 应用图标 512px
└── README.md
```

## 部署方法

### GitHub Pages（推荐）

1. 在 GitHub 创建新仓库（如 `persona-test`）
2. 上传全部文件到仓库根目录
3. 进入仓库 Settings → Pages → Source 选择 `main` 分支
4. 访问 `https://你的用户名.github.io/persona-test/`

### 其他静态托管

直接上传全部文件到任意静态托管服务即可：
- Vercel、Netlify、Cloudflare Pages 均支持

## 功能说明

- **58道题目** · 7大心理学框架
  - 大五人格 OCEAN（15题）
  - 情感依恋模式四维度（8题）
  - 认知风格（6题）
  - 情绪智力 EQ（10题）
  - 核心价值观 Schwartz（8题）
  - 心理韧性（5题）
  - 思维模式与信念（6题）

- **PWA 支持**：可安装到手机主屏幕，支持离线使用
- **深度解读**：结果页"获取深度解读报告"按钮，在 Claude.ai 中调用 Claude 深度分析
- **纯前端**：无需后端，无需 API Key，完全本地运行

## 技术栈

- 纯 HTML / CSS / JavaScript（无框架依赖）
- Chart.js 4.4.1（雷达图 + 横向条形图）
- Google Fonts：Noto Serif SC + Noto Sans SC
- PWA：Web App Manifest + Service Worker
