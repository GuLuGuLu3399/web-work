<div align="center">🚀 Web-Work 综合学习平台现代化全栈学习平台 · 算法可视化 · 在线判题 (OJ) · 沉浸式阅读功能特性 • 快速开始 • 技术架构 • 项目哲学 • 文档</div>🎯 功能特性模块功能描述📚 学习中心技术文章 (Markdown/LaTeX/图表)、在线编程(OJ) (多语言/实时编译)、算法可视化 (排序/搜索/DP)🛠️ 管理后台内容发布、层级标签管理、实时数据统计、系统配置🎨 用户体验深色/浅色模式自动切换、移动端适配、Motion-v 丝滑动画、WCAG 2.1 AA 无障碍支持🎵 摸鱼组件内置音乐播放器 (单曲循环/圆形进度条/可视化动效)🚀 快速开始环境要求Node.js: >= 18.0.0npm: >= 9.0.0Go: >= 1.20 (后端开发)安装与运行# 1. 克隆项目
git clone [https://github.com/HYH0309/web-work.git](https://github.com/HYH0309/web-work.git)
cd web-work

# 2. 安装依赖
npm install

# 3. 启动开发服务器
npm run dev
常用命令命令说明npm run build构建生产版本npm run preview预览构建结果npm run type-checkTypeScript 类型检查npm run lint代码检查与格式化node scripts/analyze-deps.js依赖体积分析📖 技术架构🏗️ 前端技术栈核心框架: Vue 3.5 (Composition API) + TypeScript 5.8 + Vite 6.3UI/样式: UnoCSS (Atomic CSS) + Headless UI + Heroicons状态管理: Pinia 3.0 + VueUse内容渲染: Markdown-it (解析) + CodeMirror 6 (编辑器) + Mermaid (图表) + KaTeX (公式)动效/测试: Motion-v + Playwright + ESLint/Prettier🔧 后端技术栈 (WIP)核心框架: Gin Web Framework数据存储: GORM + MySQL/PostgreSQL + Redis认证安全: JWT 令牌机制🎭 项目哲学 (Backend Features)<details><summary><b>点击查看：后端架构师的"绝妙"设计与自白</b></summary>"如果你永远不知道接口会返回什么，那它就是防爬虫的最佳设计。" —— 某后端架构师1. 薛定谔的 Result 结构HTTP 200 并不代表成功，一切皆有可能。type Result struct {
    Status  bool   `json:"status"` // 与HTTP状态码完美冲突
    Message string `json:"msg"`    // 自由创作的诗意空间
    Data    any    `json:"data"`   // 类型安全的终结者 (可能是对象/数组/null/字符串)
}
2. 分层架构的极致艺术HTTP → 路由 → 中间件 → 控制器 → DTO → 服务层 → 仓库层 → 数据库(实际业务逻辑占比 < 5%)3. 贡献者福利免费心理咨询券（处理类型断言焦虑）《防御性编程大师》课程如何解释 "这是一个特性不是 Bug" 的培训</details>🗺️ 发展规划[x] v1.0 前端核心: 文章展示、OJ 练习、算法可视化、管理后台、响应式设计[ ] v1.5 后端整合: Gin+GORM API、数据库设计、JWT 认证[ ] v2.0 功能扩展: SQL 可视化练习、CSS 训练、用户积分系统[ ] v3.0 智能化: AI 代码助手、多语言支持、移动端 App📂 目录结构src/
├── views/           # 页面 (Article, OJ, Visualizer, Admin)
├── components/      # 组件 (业务组件 + 通用组件)
├── composables/     # 组合式函数 (Logic Reuse)
├── stores/          # Pinia 状态管理
├── utils/           # 工具函数
└── assets/          # 静态资源
🤝 贡献与支持欢迎提交 Pull Request 或 Issue。提交代码前请确保通过 npm run type-check。📄 许可证本项目采用 MIT License 开源协议。<div align="center">Made with ❤️ by Vue Community⭐ 喜欢这个项目？请给一个 Star！</div>
