# 数据看板

基于 HTML + CSS + JavaScript 的响应式数据看板页面，支持明暗主题切换。

## 功能

- 6 张核心指标卡片：活跃用户、今日营收、订单总量、访问量、转化率、在线节点
- 每张卡片含图标、数值、环比变化（上升绿色 / 下降红色，带箭头）
- 明暗主题切换：`data-theme` 属性 + CSS 自定义属性实现
- 响应式布局：≥1200px 四列 + 侧边栏，768~1199px 两列，<768px 单列
- 卡片 hover 上移 + 阴影过渡

## 技术要点

- 内联 SVG 图标（`stroke="currentColor"`，颜色随主题切换）
- 数据驱动渲染：卡片由 `cardsData` 数组 + `map` 生成
- CSS Grid `auto-fit + minmax` 自适应，无写死宽度
- 三文件分离：`index.html` / `style.css` / `script.js`

## 预览

直接用浏览器打开 `index.html` 即可，无需安装依赖。
