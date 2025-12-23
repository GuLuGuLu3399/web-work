<div align="center">
  <h1>🚀 Web-Work 综合学习平台</h1>
  <p>现代化全栈学习平台 · 算法可视化 · 在线判题 (OJ) · 沉浸式阅读</p>
</div>

## 🎯 功能特性

| 模块 | 功能 | 描述 |
|------|------|------|
| **📚 学习中心** | 技术文章 | Markdown/LaTeX/图表支持 |
| | 在线编程 (OJ) | 多语言支持，实时编译执行 |
| | 算法可视化 | 排序/搜索/动态规划可视化 |
| **🛠️ 管理后台** | 内容管理 | 文章发布、编辑、删除 |
| | 标签系统 | 多级标签分类管理 |
| | 数据统计 | 实时用户行为分析 |
| | 系统配置 | 平台参数配置 |
| **🎨 用户体验** | 主题系统 | 深色/浅色模式自动切换 |
| | 响应式设计 | 移动端适配 |
| | 动画效果 | Motion-v 平滑过渡动画 |
| | 无障碍支持 | WCAG 2.1 AA 标准兼容 |
| **🎵 娱乐组件** | 音乐播放器 | 单曲循环，圆形进度条 |
| | 音频可视化 | 动态频谱可视化 |

## 🚀 快速开始

### 环境要求

- **Node.js**: >= 18.0.0
- **npm**: >= 9.0.0
- **Go**: >= 1.20 (后端开发)
- **数据库**: MySQL 8.0+ 或 PostgreSQL 14+

### 安装步骤

bash
1. 克隆项目

git clone https://github.com/HYH0309/web-work.git
cd web-work

2. 安装依赖

npm install

3. 配置环境变量

cp .env.example .env
编辑 .env 文件，配置数据库连接等参数

4. 启动开发服务器

npm run dev


### 常用命令

| 命令 | 说明 |
|------|------|
| `npm run build` | 构建生产版本 |
| `npm run preview` | 预览构建结果 |
| `npm run type-check` | TypeScript 类型检查 |
| `npm run lint` | 代码检查与格式化 |
| `npm run test` | 运行单元测试 |
| `node scripts/analyze-deps.js` | 依赖体积分析 |

## 📖 技术架构

### 🏗️ 前端技术栈

| 分类 | 技术选型 | 说明 |
|------|----------|------|
| **核心框架** | Vue 3.5 + TypeScript 5.8 | Composition API 开发模式 |
| **构建工具** | Vite 6.3 | 现代化构建工具 |
| **样式方案** | UnoCSS + Tailwind CSS | 原子化 CSS 框架 |
| **UI 组件** | Headless UI + Heroicons | 无头 UI 组件库 |
| **状态管理** | Pinia 3.0 + VueUse | 现代化状态管理 |
| **内容渲染** | Markdown-it + CodeMirror 6 | Markdown 解析与编辑器 |
| **图表渲染** | Mermaid + KaTeX | 流程图与数学公式 |
| **动效方案** | Motion-v + Framer Motion | 平滑动画效果 |
| **测试框架** | Playwright + Vitest | E2E 测试与单元测试 |
| **代码质量** | ESLint + Prettier | 代码规范与格式化 |

### 🔧 后端技术栈 (开发中)

| 分类 | 技术选型 | 说明 |
|------|----------|------|
| **核心框架** | Gin Web Framework | 高性能 Go Web 框架 |
| **数据库 ORM** | GORM 2.0 | 现代化 ORM 框架 |
| **数据存储** | MySQL/PostgreSQL + Redis | 关系型数据库 + 缓存 |
| **认证授权** | JWT + Casbin | 令牌认证与权限控制 |
| **API 文档** | Swagger/OpenAPI 3.0 | API 接口文档 |
| **消息队列** | RabbitMQ/Kafka | 异步任务处理 |
| **监控日志** | Prometheus + Grafana | 系统监控与可视化 |
| **容器化** | Docker + Docker Compose | 容器化部署 |

## 🎭 项目哲学

<details>
<summary><b>点击查看：后端架构设计理念</b></summary>

### 1. 确定性的 API 设计
typescript
// 统一的响应格式
interface ApiResponse<T> {
  code: number;      // 业务状态码
  message: string;   // 友好的提示信息
  data: T;           // 类型安全的数据负载
  timestamp: number; // 响应时间戳
  requestId: string; // 请求追踪 ID
}


### 2. 清晰的分层架构

HTTP → 路由层 → 中间件层 → 控制器层 → 服务层 → 数据访问层 → 数据库
         ↓           ↓           ↓         ↓         ↓          ↓
    请求验证     权限控制     参数解析   业务逻辑   数据操作   持久化存储


### 3. 开发者友好特性
- **完整的 TypeScript 类型定义**
- **详细的 API 文档与示例**
- **完整的错误码枚举**
- **开发环境热重载支持**
- **集成测试与 E2E 测试**

### 4. 性能与扩展性
- **数据库连接池优化**
- **Redis 缓存策略**
- **API 响应压缩**
- **CDN 静态资源分发**
- **水平扩展支持**
</details>

## 🗺️ 发展规划

### v1.0 基础版 (已完成)
- [x] 前端核心框架搭建
- [x] 文章展示与编辑功能
- [x] OJ 在线判题系统
- [x] 算法可视化组件
- [x] 响应式设计与主题系统
- [x] 管理后台基础功能

### v1.5 后端整合版 (进行中)
- [ ] Gin + GORM API 服务开发
- [ ] 数据库设计与迁移脚本
- [ ] JWT 认证与权限系统
- [ ] RESTful API 规范制定
- [ ] 前端后端数据对接

### v2.0 功能扩展版 (计划中)
- [ ] SQL 可视化练习平台
- [ ] CSS 交互式训练场
- [ ] 用户积分与等级系统
- [ ] 社交功能（评论/点赞/分享）
- [ ] 学习进度跟踪

### v3.0 智能化版 (规划中)
- [ ] AI 代码助手与智能提示
- [ ] 多语言国际化支持
- [ ] 移动端原生应用
- [ ] 离线学习功能
- [ ] 个性化学习推荐

## 📂 项目结构


web-work/
├── src/                    # 前端源代码
│   ├── views/             # 页面组件
│   │   ├── Article/       # 文章页面
│   │   ├── OJ/           # 在线判题页面
│   │   ├── Visualizer/   # 算法可视化页面
│   │   └── Admin/        # 管理后台页面
│   ├── components/        # 可复用组件
│   │   ├── common/       # 通用组件
│   │   └── business/     # 业务组件
│   ├── composables/       # Composition API 函数
│   ├── stores/           # Pinia 状态管理
│   ├── utils/            # 工具函数库
│   ├── assets/           # 静态资源
│   └── types/            # TypeScript 类型定义
├── server/                # 后端服务
│   ├── api/              # API 接口层
│   ├── service/          # 业务逻辑层
│   ├── dao/              # 数据访问层
│   ├── model/            # 数据模型
│   ├── middleware/       # 中间件
│   └── config/           # 配置文件
├── docs/                  # 项目文档
├── scripts/              # 构建脚本
├── tests/                # 测试文件
├── docker/               # Docker 配置
└── config/               # 构建配置


## 🤝 贡献指南

### 提交代码流程

1. **Fork 项目仓库**
2. **创建功能分支**
   bash
   git checkout -b feat/your-feature-name

3. **提交代码变更**
   bash
   git add .
   git commit -m "feat: add your feature"

4. **推送到远程仓库**
   bash
   git push origin feat/your-feature-name

5. **创建 Pull Request**

### 开发规范

- 遵循 **Conventional Commits** 提交规范
- 提交前运行 `npm run lint` 和 `npm run type-check`
- 新功能需要补充单元测试
- API 变更需要更新接口文档
- UI 变更需要适配移动端

### 问题反馈

- 使用 [GitHub Issues](https://github.com/HYH0309/web-work/issues) 报告问题
- 提供清晰的问题描述和复现步骤
- 对于功能建议，请描述使用场景和预期效果

## 📄 许可证

本项目采用 **MIT License** 开源协议。详见 [LICENSE](LICENSE) 文件。

<div align="center">
  <p>Made with ❤️ by Vue Community</p>
  <p>⭐ 喜欢这个项目？请给一个 Star！</p>
</div>
