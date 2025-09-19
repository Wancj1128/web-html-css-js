# 零基础前端学习计划（Vue 路线｜纯 CSS｜12周）

适用对象：从零开始的前端学习者  
技术栈：Vue 3 + Vite + Vue Router + Pinia + Vitest + Testing Library（样式使用纯 CSS，不用 Tailwind/Styled Components）  
学习强度：每周 12 小时（配套 4×3h 日程在 frontend-study-schedule-12h-4x3h.md）  
输出要求：每周 1 个可运行 Demo（附在线链接）+ README 复盘

---

## 总览路线图（Vue + 纯 CSS）

1) 基础三件套
- HTML：语义化、表单、媒体、基础可访问性
- CSS（纯 CSS）：选择器、盒模型、Flexbox/Grid、响应式、CSS 变量、媒体查询、过渡与动画
- JS：语法、作用域/闭包、原型、DOM、事件、异步（Promise/async）、模块化

2) 浏览器与网络
- DevTools 调试与性能面板
- HTTP/HTTPS、缓存策略、CORS、Cookie/Storage、安全（XSS/CSRF/CSP）

3) 工程化
- Node.js、npm（或 pnpm）
- Vite 脚手架与环境变量
- Git/GitHub 工作流、ESLint + Prettier

4) Vue 生态
- Vue 3（组合式 API）、组件化、props/emit、受控表单、插槽
- Vue Router（嵌套路由、动态路由、导航守卫）
- Pinia（state/getters/actions、模块化、可选持久化）
- 样式：纯 CSS（BEM 命名 + CSS 变量 + 媒体查询；可选 CSS Modules）

5) 质量与体验
- 测试（Vitest + Vue Testing Library）
- 可访问性（a11y）
- 性能优化（代码分割、懒加载、图片优化）

6) 进阶
- TypeScript（在 Vue/Pinia/Router 中落地）
- 认证（JWT/OAuth）与前端安全
- 部署（Vercel/Netlify/GitHub Pages）

---

## 周计划（12周）

> 每周执行："学 → 做 → 交付 → 复盘"，保持最小可用产品输出。

### 第1周：HTML + CSS 入门（纯 CSS）
- 学：语义化标签、表单与输入类型；CSS 选择器、盒模型、常用单位（px/%/rem）
- 做：移动端优先的一页简历/名片
- 交付：语义化 + 响应式的单页（含在线链接）

### 第2周：布局与响应式
- 学：Flexbox、Grid、媒体查询、响应式图片
- 做：产品落地页（Hero/Features/Pricing/Footer）
- 交付：手机与桌面均表现良好

### 第3周：JavaScript 基础
- 学：变量/类型、数组/对象、函数、this/箭头函数、模块化初识
- 做：交互组件小合集（计时器/轮播/Tab）
- 交付：原生 JS 交互组件集

### 第4周：DOM、事件与数据处理
- 学：DOM 操作、事件委托、表单校验、节流/防抖、JSON
- 做：Todo App（增删改查 + LocalStorage）
- 交付：可用的 Todo 应用

### 第5周：异步与网络请求
- 学：Fetch、Promise/async、错误处理、CORS、简单缓存策略
- 做：公共 API 搜索（搜索/分页/加载与错误态）
- 交付：API 搜索应用

### 第6周：工程化与协作
- 学：Node、npm、Vite、环境变量、ESLint/Prettier、Git 分支与 PR
- 做：将第5周项目迁移到 Vite；建立 lint/format/build 脚本
- 交付：工程化重构后的项目 + 使用说明

### 第7周：Vue 3 入门（组合式 API）
- 学：Vite + Vue 初始化、模板语法、ref/reactive、computed、watch、组件/props/emit、插槽
- 做：组件练习（按钮/Input/对话框/通知）
- 交付：3–5 个可复用组件（配纯 CSS 样式）

### 第8周：路由与状态管理
- 学：Vue Router（嵌套/动态/守卫）；Pinia（state/getters/actions、模块化）
- 做：小型 SPA（多视图 + 守卫 + 全局状态）
- 交付：带路由与全局状态的应用

### 第9周：纯 CSS 设计体系与主题
- 学：BEM 命名、CSS 变量（设计令牌：颜色/间距/字号）、媒体查询、prefers-color-scheme、过渡/动画
- 做：为第8周项目统一样式系统；实现浅/深色主题切换（仅用 CSS 变量）
- 交付：统一视觉 + 主题切换的 SPA

### 第10周：测试、可访问性与性能
- 学：Vitest + Vue Testing Library、a11y（语义/对比度/键盘导航）、性能（代码分割/图片懒加载）
- 做：编写组件与 store 测试；跑 Lighthouse 并优化
- 交付：核心模块测试覆盖 >60% + Lighthouse 合格

### 第11周：TypeScript 实战
- 学：基础类型、接口、泛型、类型推断；在 Vue/Pinia/Router 中落地
- 做：将第8–9周项目核心模块迁移到 TS（组件 props/事件、store 类型）
- 交付：严格模式构建通过、类型无报错

### 第12周：综合实战与发布
- 做：电商迷你站/课程平台/看板（三选一）
  - 路由 + 状态 + API + 认证（模拟或简单后端）
  - 表单校验与错误、a11y、性能优化
- 交付：部署到 Vercel/Netlify，并写技术文档

---

## 纯 CSS 实施建议

- 结构化命名：BEM（block__element--modifier）
- 设计令牌：用 :root 定义 --color-primary、--spacing-sm、--font-size-base 等
- 主题切换：html[data-theme="dark"] 覆盖 CSS 变量；或使用 @media (prefers-color-scheme: dark)
- 响应式：移动端优先；使用 clamp() 进行流式字号/间距；媒体查询断点按内容需要设置
- 动效：transition/transform 为主，避免大范围 box-shadow 与昂贵动画

---

## Vue 技术栈与工具

- 脚手架：Vite（模板：vue）
- 路由：Vue Router
- 状态：Pinia（可选持久化插件）
- 样式：纯 CSS（必要时可用 CSS Modules，但不引入 Tailwind/SC）
- HTTP：fetch 或 axios（二选一）
- 测试：Vitest + Vue Testing Library
- Lint：ESLint（eslint-plugin-vue）+ Prettier
- VS Code 扩展：Volar、ESLint、Prettier、Auto Rename Tag、GitLens

---

## 快速起步（预览）

```bash
# 新建项目
npm create vite@latest my-vue-app -- --template vue
cd my-vue-app
npm install
npm run dev

# ESLint + Prettier（JS 版本）
npm i -D eslint eslint-plugin-vue @vue/eslint-config-prettier prettier

# Vue Router / Pinia
npm i vue-router pinia

# 测试
npm i -D vitest @vitejs/plugin-vue @vue/test-utils @testing-library/vue jsdom
```

---

## 自测清单

- [ ] HTML/CSS：语义化、表单、盒模型、Flex/Grid、响应式、CSS 变量/主题
- [ ] JS：作用域/闭包、DOM/事件、Promise/async、模块化、错误处理
- [ ] 浏览器与网络：DevTools、HTTP/CORS/缓存、存储与安全
- [ ] 工程化：Vite、环境变量、ESLint/Prettier、Git 工作流
- [ ] Vue 生态：组合式 API、组件通信、路由、Pinia
- [ ] 质量与进阶：测试、a11y、性能优化、TypeScript、部署