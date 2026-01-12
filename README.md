# OKly - 全平台加密货币智能交易系统

<div align="center">

**OKly** 是一个功能完整的加密货币自动交易系统，支持macOS、Web和微信小程序三大平台。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/platform-macOS%20%7C%20Web%20%7C%20Miniprogram-blue.svg)](https://github.com/chenlaiyi/OKly)

[特性](#-特性) • [快速开始](#-快速开始) • [技术栈](#-技术栈) • [文档](#-文档) • [许可证](#-许可证)

</div>

---

## 📖 项目简介

OKly是一个专业的加密货币自动交易系统，集成了实时行情监控、AI智能分析、策略配置、自动交易等完整功能。

### 支持平台

- 🖥️ **macOS桌面端** - 原生Swift应用，功能最完整
- 🌐 **Web浏览器端** - 在线交易平台，随时随地访问
- 📱 **微信小程序** - 移动端便捷交易

---

## ✨ 核心特性

### 📊 实时行情监控
- 支持多个交易对的实时行情显示
- K线图表展示（1H、4H、1D周期）
- 技术指标分析（SAR、MACD、RSI等）

### 🤖 AI智能分析
- 基于智谱AI的市场分析
- 交易建议和风险评估
- 置信度评分系统

### ⚙️ 策略配置
- 灵活的交易策略配置系统
- 支持多指标组合（SAR、MACD等）
- 自定义买入卖出条件
- 资金管理和风险控制设置

### 🔄 自动交易
- 策略自动执行交易
- 实时持仓监控
- 止盈止损自动触发
- 冷却机制和风险控制

### 💼 持仓管理
- 实时持仓列表
- 未实现盈亏计算
- 交易历史记录
- 统计分析报表

---

## 🚀 快速开始

### macOS端

1. 下载最新版本
2. 打开 `Okly.app`
3. 配置OKX API密钥
4. 开始交易

详细文档请查看 [macOS/README.md](./macOS/README.md)

### Web端

访问在线平台：[https://ly.ddg.org.cn](https://ly.ddg.org.cn)

功能包括：
- 实时行情和K线图
- AI分析建议
- 在线交易执行
- 策略配置管理

### 微信小程序

1. 打开微信开发者工具
2. 导入 `miniprogram` 目录
3. 编译运行
4. 扫码体验

详细文档请查看 [miniprogram/README.md](./miniprogram/README.md)

---

## 🔧 技术栈

### macOS端
- **语言**: Swift 5.9+
- **框架**: SwiftUI, Combine
- **架构**: MVVM
- **依赖**: Swift Package Manager

### Web端
- **后端**: Node.js, Express
- **数据库**: MySQL
- **前端**: 纯HTML/CSS/JavaScript
- **图表**: Lightweight Charts
- **实时通信**: WebSocket (ws)

### 小程序端
- **框架**: 微信小程序原生
- **语言**: TypeScript
- **样式**: Less
- **API**: REST + WebSocket

---

## 📁 项目结构

\`\`\`
OKly/
├── macOS/              # macOS桌面端
│   ├── Sources/        # Swift源代码
│   ├── Okly.app/       # 应用程序
│   └── README.md       # macOS端文档
│
├── web/                # Web端（部署在服务器）
│   ├── backend/        # Node.js后端
│   ├── frontend/       # Web前端
│   └── README.md       # Web端文档
│
├── miniprogram/        # 微信小程序
│   ├── pages/          # 页面
│   ├── services/       # API服务
│   ├── models/         # 数据模型
│   └── README.md       # 小程序端文档
│
├── docs/               # 共享文档
│   ├── API.md          # API文档
│   ├── DATABASE.md     # 数据库设计
│   └── DEVELOPMENT.md  # 开发文档
│
└── README.md           # 本文件
\`\`\`

---

## 📊 功能对比

| 功能 | macOS端 | Web端 | 小程序端 | 完成度 |
|------|---------|-------|----------|--------|
| 实时行情 | ✅ | ✅ | ✅ | 100% |
| K线图表 | ✅ | ✅ | ⏳ | 90% |
| AI分析 | ✅ | ✅ | ✅ | 100% |
| 策略配置 | ✅ | ✅ | ⏳ | 85% |
| 自动交易 | ✅ | ✅ | ✅ | 100% |
| 持仓管理 | ✅ | ✅ | ✅ | 100% |
| 交易历史 | ✅ | ✅ | ✅ | 100% |
| 账号管理 | ✅ | ⏳ | ⏳ | 70% |

---

## 🛠️ 开发指南

### macOS端开发

\`\`\`bash
cd macOS
xcodebuild -project OKly.xcodeproj
open Okly.app
\`\`\`

### Web端开发

\`\`\`bash
cd web/backend
npm install
pm2 start server.js
\`\`\`

### 小程序端开发

\`\`\`bash
cd miniprogram
npm install
# 在微信开发者工具中打开项目
\`\`\`

---

## 📝 更新日志

### v1.0.0 (2026-01-12)

#### 新增功能
- ✅ macOS端完整策略配置系统
- ✅ Web端在线交易平台
- ✅ 微信小程序端基础框架
- ✅ AI智能分析集成
- ✅ 实时行情数据对接

#### 技术改进
- ✅ TypeScript类型安全
- ✅ MVVM架构优化
- ✅ API服务层封装
- ✅ 数据库集成方案

---

## 🤝 贡献指南

欢迎贡献代码！请查看各端的开发文档。

### 开发流程

1. Fork本仓库
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启Pull Request

---

## 📄 开源协议

本项目采用 **MIT协议** 开源。

---

## 🙏 致谢

感谢以下开源项目和服务：

- [Swift](https://swift.org) - 苹果开源编程语言
- [Node.js](https://nodejs.org) - JavaScript运行时
- [Lightweight Charts](https://www.tradingview.com/lightweight-charts/) - 金融图表库
- [智谱AI](https://open.bigmodel.cn/) - AI分析服务
- [OKX](https://www.okx.com) - 加密货币交易所

---

<div align="center">

**Made with ❤️ by OKly Team**

[⭐ Star](https://github.com/chenlaiyi/OKly) this repo if you like it!

[🐛 Report Bug](https://github.com/chenlaiyi/OKly/issues) · 💡 [Request Feature](https://github.com/chenlaiyi/OKly/issues)

</div>
