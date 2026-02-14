# ToyCraftLauncher

一个正在开发中的 Minecraft 启动器喵~

## 项目简介

本项目是一个基于 Tauri 2 + Vue 3 + Vite 开发的桌面应用程序喵~

## 技术栈

| 层级 | 技术 |
|------|------|
| 前端 | Vue 3 + TypeScript + Vite |
| 后端 | Rust + Tauri 2 |
| 构建工具 | npm |

## 项目结构

```
ToyCraftLauncher/
├── src/                    # 前端代码 (Vue 3)
│   ├── main.ts            # 前端入口
│   ├── App.vue            # 主组件
│   └── assets/            # 静态资源
├── src-tauri/             # 后端代码 (Rust)
│   ├── src/
│   │   ├── lib.rs         # Tauri 命令定义
│   │   └── main.rs        # 后端入口
│   ├── Cargo.toml         # Rust 依赖配置
│   └── tauri.conf.json    # Tauri 配置
├── package.json           # 前端依赖配置
├── vite.config.ts         # Vite 配置
└── tsconfig.json          # TypeScript 配置
```

## 快速开始

### 前置要求

- Node.js (LTS 版本)
- Rust (最新版)
- npm 或 pnpm

### 安装依赖

```bash
npm install
```

### 开发模式

```bash
# 启动前端开发服务器
npm run dev

# 启动 Tauri 开发模式
npm run tauri dev
```

### 构建发布

```bash
npm run tauri build
```

## 功能规划

- [ ] 启动器主界面
- [ ] 游戏版本管理
- [ ] 登录验证
- [ ] 配置文件管理

## 开发说明

- 前端代码位于 `src/` 目录，使用 Vue 3 编写喵~
- 后端代码位于 `src-tauri/src/` 目录，使用 Rust 编写喵~
- 前端与后端通过 Tauri 的 `invoke` 命令进行通信喵~

## 相关文档

- [Tauri 文档](https://tauri.app/zh-cn/v1/)
- [Vue 3 文档](https://vuejs.org/)
- [Vite 文档](https://vitejs.dev/)

