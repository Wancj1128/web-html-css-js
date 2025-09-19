# 12 小时/周学习日程（4×3h 模式｜Vue 路线｜纯 CSS）

说明
- 模式：每周 4 次，每次 3 小时（建议固定 4 天，如 Tue/Thu/Sat/Sun）
- 方法：每次学习都进行"学 → 做 → 交付 → 复盘"，坚持小步快跑
- 交付：每周至少 1 个可运行 Demo（含在线部署链接）+ README 复盘

每次 3 小时建议结构
- 专注 65min × 2 + 10min 休息
- 复盘与提交 20–30min
- 机动缓冲 10–20min（查文档/微调样式）

---

## 固定周节奏（适用于 12 周）

- Session A（3h）学习与计划
  - 阅读 MDN/文档，做要点摘记
  - 制定本周任务清单与验收标准
- Session B（3h）基础练习
  - 针对本周关键点做 1–2 个小练习
- Session C（3h）项目主功能
  - 实现核心功能 A（最小可用版本）
- Session D（3h）打磨与交付
  - 实现功能 B；可访问性与细节；部署与复盘

Tips
- 每周至少 4 次提交：feat/bugfix/docs/refactor 分类清晰
- 优先保证"能用+可部署"，再持续打磨样式与体验

---

## 第1周（HTML + 纯 CSS 入门，12h）

目标
- 掌握语义化标签、表单基础、CSS 选择器与盒模型、常用单位（px/%/rem）
- 交付：移动端优先的一页简历/名片（语义化 + 响应式）

Session A（3h）学习与计划
- 学习：MDN（HTML 语义/表单、CSS 选择器/盒模型/display）
- 输出：摘记与速查清单；本周任务与标准
- 验收：提交 docs/notes/week1.md，列出关键概念与示例

Session B（3h）基础练习
- 练习 1：语义化结构（header/main/section/footer）
- 练习 2：卡片组件（含图片/标题/按钮，hover 状态）
- 练习 3：响应式图片（img + srcset/sizes）
- 验收：/practice/week1 下 2–3 个最小页面，代码通过校验

Session C（3h）项目主功能
- 项目：个人名片/简历单页（移动端优先）
- 实现：信息结构、基础排版、颜色/间距体系
- 验收：375px 视口无水平滚动，导航/锚点可用

Session D（3h）打磨与交付
- 增强：表单联络区（label/placeholder/必填校验）、按钮状态、链接可见性
- a11y：图片 alt、表单 label、颜色对比
- 部署：GitHub Pages/Netlify/Vercel；README 附在线链接与截图
- 验收标准：
  - 语义化合理（header/main/section/footer/ul/label/alt）
  - 响应式在 375/768/1024 正常、无水平滚动
  - Lighthouse a11y ≥ 90（静态页通常可达）
  - 交付：在线链接 + 源码 + README

---

## 第2周（布局与响应式，12h）

目标
- 掌握 Flexbox、Grid、媒体查询与响应式图片
- 交付：产品落地页（Hero/Features/Pricing/CTA/Footer），手机与桌面表现良好

Session A（3h）学习与计划
- 学习：Flex 容器/项目属性、Grid 模板/区域命名、媒体查询
- 输出：布局速查与常见布局草图；本周任务与标准
- 验收：提交 docs/notes/week2.md

Session B（3h）基础练习
- Flex：导航栏（左右对齐）、三列信息条
- Grid：杂志式区块（header/aside/main/footer）
- 验收：/practice/week2 下 2–3 个布局示例

Session C（3h）项目主功能
- 页面：搭建落地页结构与 Hero/Features 区块（移动端优先）
- 验收：主要区块在 375px 完整显示，排版清晰

Session D（3h）打磨与交付
- 完成：Pricing 卡片、CTA、Footer；桌面端断点布局
- 性能：响应式图片 srcset/sizes、图片延迟加载；Lighthouse 测试
- 验收标准：
  - Flex/Grid 使用恰当，元素对齐合理
  - 至少两个断点（<=640、>=1024）排版优
  - Lighthouse Performance ≥ 90（静态页通常可达）
  - 交付：在线链接 + 源码 + README（含断点策略与得分截图）

---

## 第3周（JavaScript 基础，12h）— 概要

- 学：变量/类型、数组/对象、函数、this/箭头函数、模块化初识
- 项目：交互组件小合集（计时器/轮播图/Tab）
- 节奏：按 4×3h 模板执行（如需我可出逐 Session 清单）

---

## 第4周（DOM/事件/数据处理，12h）— 概要

- 学：DOM 操作、事件委托、表单校验、节流/防抖、JSON
- 项目：Todo App（LocalStorage 增删改查）
- 节奏：按 4×3h 模板执行（如需我可出逐 Session 清单）

---

后续周次
- 第5–12周按 frontend-study-plan-vue.md 的主题推进
- 若需要，我可以为每一周生成"逐 Session（3h）任务 + 验收标准 + 资料链接"