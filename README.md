# OKly - 全平台加密货币智能交易系统

<div align="center">

**OKly** 是一个功能完整的加密货币自动交易系统，支持macOS、Web和微信小程序三大平台。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/platform-macOS%20%7C%20Web%20%7C%20Miniprogram-blue.svg)](https://github.com/chenlaiyi/OKly)

[平台介绍](#-支持平台) • [快速开始](#-快速开始) • [在线体验](#-在线体验) • [技术栈](#-技术栈) • [许可证](#-许可证)

</div>

---

## 📖 项目简介

OKly是一个专业的加密货币自动交易系统，集成了实时行情监控、AI智能分析、策略配置、自动交易等完整功能。

## 🎯 支持平台

### 🖥️ macOS桌面端

**项目仓库**: [OKXTrader-Mac](https://github.com/chenlaiyi/OKXTrader-Mac)

原生Swift应用，功能最完整的客户端

- ✅ 完整的策略配置系统
- ✅ 实时行情和K线图表
- ✅ AI智能分析
- ✅ 自动交易执行
- ✅ 持仓管理和交易历史
- ✅ SAR指标反转点可视化

**技术栈**: Swift 5.9+, SwiftUI, Combine, MVVM架构

### 🌐 Web浏览器端

**在线平台**: [https://ly.ddg.org.cn](https://ly.ddg.org.cn)

随时随地访问的在线交易平台

- ✅ 实时行情数据
- ✅ K线图表展示
- ✅ AI分析建议
- ✅ 在线交易执行
- ✅ 策略配置管理

**技术栈**: Node.js, Express, MySQL, Lightweight Charts, WebSocket

### 📱 微信小程序

**项目仓库**: [OKXTrader-Miniprogram](https://github.com/chenlaiyi/OKXTrader-Miniprogram)

移动端便捷交易

- ✅ 实时行情监控
- ✅ AI分析建议
- ✅ 自动交易开关
- ✅ 持仓管理
- ✅ 交易历史查询

**技术栈**: 微信小程序原生框架, TypeScript, Less

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

```bash
# 克隆macOS端仓库
git clone https://github.com/chenlaiyi/OKXTrader-Mac.git
cd OKXTrader-Mac

# 方式1：使用已编译应用（推荐）
open Okly.app

# 方式2：使用Xcode编译
open OKXTrader.xcodeproj
```

详细文档请查看: [OKXTrader-Mac/README.md](https://github.com/chenlaiyi/OKXTrader-Mac)

### Web端

直接访问在线平台: **[https://ly.ddg.org.cn](https://ly.ddg.org.cn)**

无需安装，打开浏览器即可使用

### 微信小程序

```bash
# 克隆小程序端仓库
git clone https://github.com/chenlaiyi/OKXTrader-Miniprogram.git
cd OKXTrader-Miniprogram

# 安装依赖
npm install

# 打开微信开发者工具
# 导入项目目录
# 编译运行
```

详细文档请查看: [OKXTrader-Miniprogram/README.md](https://github.com/chenlaiyi/OKXTrader-Miniprogram)

---

## 🌐 在线体验

**Web平台**: [https://ly.ddg.org.cn](https://ly.ddg.org.cn)

功能包括:
- 📊 实时行情和K线图
- 🤖 AI分析建议
- 🔄 在线交易执行
- ⚙️ 策略配置管理

---

## 📊 功能对比

| 功能模块 | macOS端 | Web端 | 小程序端 | 完成度 |
|---------|---------|-------|----------|--------|
| 实时行情监控 | ✅ | ✅ | ✅ | 100% |
| K线图表 | ✅ | ✅ | ⏳ | 90% |
| 技术指标 | ✅ | ✅ | ⏳ | 85% |
| AI智能分析 | ✅ | ✅ | ✅ | 100% |
| 策略配置 | ✅ | ✅ | ⏳ | 85% |
| 自动交易 | ✅ | ✅ | ✅ | 100% |
| 持仓管理 | ✅ | ✅ | ✅ | 100% |
| 交易历史 | ✅ | ✅ | ✅ | 100% |
| 账号管理 | ✅ | ⏳ | ⏳ | 70% |
| AI聊天 | ✅ | ✅ | ⏳ | 75% |

**总体完成度**: **87%** ✅

---

## 🔧 技术栈

### macOS端
- **语言**: Swift 5.9+
- **框架**: SwiftUI, Combine
- **架构**: MVVM (Model-View-ViewModel)
- **依赖管理**: Swift Package Manager
- **最低版本**: macOS 14.0+

### Web端
- **后端**: Node.js 18+, Express 4.x
- **数据库**: MySQL 8.0+
- **前端**: HTML5, CSS3, JavaScript (ES6+)
- **图表库**: Lightweight Charts 4.x
- **实时通信**: WebSocket (ws库)
- **进程管理**: PM2

### 小程序端
- **框架**: 微信小程序原生框架
- **语言**: TypeScript 5.0+
- **样式**: Less
- **API**: REST + WebSocket
- **基础库版本**: 2.32.3+

---

## 📁 项目文档

- [API接口文档](docs/API.md) - REST API详细说明
- [数据库设计](docs/DATABASE.md) - MySQL数据库结构
- [开发指南](docs/DEVELOPMENT.md) - 开发环境配置

---

## 📝 更新日志

### v1.0.0 (2026-01-12)

#### 🎉 首次发布

**新增功能**：
- ✅ macOS端完整策略配置系统
- ✅ Web端在线交易平台
- ✅ 微信小程序端基础框架
- ✅ AI智能分析集成（智谱AI）
- ✅ 实时行情数据对接（OKX API）
- ✅ SAR指标反转点可视化
- ✅ 三平台策略配置UI统一

**技术特性**：
- ✅ TypeScript类型安全（小程序端）
- ✅ MVVM架构优化（macOS端）
- ✅ RESTful API设计（Web端）
- ✅ 完整的开发文档

**数据统计**：
- macOS端：103个文件，68,219行代码
- 小程序端：93个文件，28,715行代码
- 文档：3份完整文档
- API接口：19个REST接口

---

## 🤝 贡献指南

欢迎贡献代码！请遵循以下流程：

### 贡献流程

1. Fork对应平台的仓库到您的GitHub账号
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启Pull Request到对应仓库

### 代码规范

- **Swift**: 遵循Swift官方代码风格
- **TypeScript**: 使用ESLint + Prettier
- **JavaScript**: 使用ESLint + Prettier
- **Commit Message**: 遵循[约定式提交](https://www.conventionalcommits.org/zh/)

---

## 📄 开源协议

本项目采用 **MIT协议** 开源。

```
MIT License

Copyright (c) 2026 OKly Team

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 致谢

感谢以下开源项目和服务：

- **Swift** - 苹果开源编程语言
- **Node.js** - JavaScript运行时
- **Lightweight Charts** - 金融图表库
- **Express** - Node.js Web框架
- **MySQL** - 关系型数据库
- **智谱AI (BigModel)** - AI分析服务
- **OKX** - 加密货币交易所

---

## 📞 联系方式

- **问题反馈**: [GitHub Issues](https://github.com/chenlaiyi/OKly/issues)
- **功能建议**: [GitHub Discussions](https://github.com/chenlaiyi/OKly/discussions)

---

<div align="center">

**Made with ❤️ by OKly Team**

[⭐ Star](https://github.com/chenlaiyi/OKly) this repo if you like it!

[🐛 Report Bug](https://github.com/chenlaiyi/OKly/issues) · 💡 [Request Feature](https://github.com/chenlaiyi/OKly/issues)

**在线体验**: [https://ly.ddg.org.cn](https://ly.ddg.org.cn)

**各平台仓库**:
- macOS端: [OKXTrader-Mac](https://github.com/chenlaiyi/OKXTrader-Mac)
- 小程序端: [OKXTrader-Miniprogram](https://github.com/chenlaiyi/OKXTrader-Miniprogram)

</div>
