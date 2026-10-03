


# Midb-Manager 官方文档

![Version](https://img.shields.io/badge/version-1.0.3-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

一个轻量级的前端数据管理系统，支持数据的增删改查、本地存储和自定义 `.midb` 文件格式的导入导出。

## ✨ 特性

- 🗃️ **数据管理** - 完整的 CRUD 操作（增删改查）
- 💾 **本地存储** - 基于浏览器 localStorage，数据安全不上传
- 📁 **自定义格式** - 专用的 `.midb` 文件格式，易于识别和管理  
- 🚀 **零依赖** - 纯前端实现，无需后端服务
- 📱 **响应式设计** - 适配各种设备屏幕

## 🛠️ 安装

### 全局安装（推荐）

```bash
npm install -g midb-manager
```

### 本地安装

```bash
npm install midb-manager
```

## 🚀 快速开始

### 方法一：命令行启动（最简单）

```bash
# 全局安装后
midb-manager

# 或本地安装后  
npx midb-manager
```

### 方法二：使用 npm 脚本

```bash
# 进入项目目录
cd node_modules/midb-manager

# 启动本地服务器（推荐，避免 CORS 问题）
npm run serve

# 或直接打开
npm start
```

### 方法三：手动打开

```bash
cd node_modules/midb-manager
# 双击 index.html 或使用浏览器打开
```

## 📖 使用指南

### 基本操作

1. **添加数据** - 在表单中输入名称和数值，点击"添加数据"
2. **查看数据** - 所有数据以表格形式展示在下方
3. **删除数据** - 点击每条数据右侧的"删除"按钮
4. **清空数据** - 点击"清空数据"按钮清空所有记录

### 文件操作

- **导出数据** - 点击"导出数据 (.midb)"将数据保存为 `.midb` 文件
- **导入数据** - 点击"导入数据 (.midb)"从文件恢复数据
- **格式兼容** - 支持 `.midb` 和 `.json` 格式文件

## 🔧 技术细节


### 数据存储

- 使用浏览器 localStorage 进行数据持久化
- 支持跨会话数据保存
- 单文件最大支持 5MB 数据

## 📁 项目结构

```
midb-manager/
├── index.html          # 主页面
├── package.json        # 项目配置
├── bin/
│   └── cli.js          # 命令行入口
└── assets/
    └── style.css       # 样式文件
```

## 🐛 故障排除

### 常见问题

1. **页面空白** - 使用 `npm run serve` 启动本地服务器避免 CORS 问题
2. **导入失败** - 确保文件格式正确，支持 `.midb` 和 `.json`
3. **数据丢失** - 定期导出备份，数据仅存储在本地

### 获取帮助

如遇问题，请：

1. 检查浏览器控制台错误信息（F12）
2. 确保使用最新版本
3. 提交 [Issue](https://github.com/your-repo/midb-manager/issues)

## 📄 许可证

MIT License © 2025 [董翔]

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

**温馨提示**：建议使用 `npm run serve` 启动以获得最佳体验，避免文件协议的限制问题。