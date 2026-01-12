# OKly 开发文档

## 开发环境设置

### macOS端
- Xcode 15.0+
- Swift 5.9+
- macOS 14.0+

### Web端
- Node.js 18+
- MySQL 8.0+
- PM2 进程管理

### 小程序端
- 微信开发者工具
- TypeScript 5.0+

## 代码仓库

- **GitHub**: https://github.com/chenlaiyi/OKly
- **License**: MIT

## 分支策略

- `main` - 生产环境
- `develop` - 开发环境
- `feature/*` - 功能分支

## 提交规范

\`\`\`
feat: 新功能
fix: 修复bug
docs: 文档更新
style: 代码格式调整
refactor: 重构
test: 测试
chore: 构建/工具链更新
\`\`\`

## 发布流程

1. 更新版本号
2. 更新CHANGELOG
3. 创建git tag
4. 推送到GitHub
5. 发布各平台版本
