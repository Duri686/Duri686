<h1 align="center">Hi, I'm Duri 👋</h1>

<p align="center">
  F2E Engineer · Web Visualization (WebGL/Three.js, PixiJS) · A* Pathfinding & Multi-floor Routing · Vite/TS · Web Workers · Actions
</p>

<p align="center">
  <a href="https://github.com/Duri686"><img src="https://komarev.com/ghpvc/?username=Duri686&color=0ea5e9&style=for-the-badge" alt="views" /></a>
  <a href="https://github.com/Duri686?tab=followers"><img src="https://img.shields.io/github/followers/Duri686?style=for-the-badge" alt="followers" /></a>
  <a href="https://github.com/Duri686?tab=repositories&sort=stargazers"><img src="https://img.shields.io/github/stars/Duri686?style=for-the-badge" alt="stars" /></a>
</p>

## 👨‍💻 关于我
- **核心领域**: 2D/3D 地图可视化 (Leaflet, Three.js), 室内导航与路径规划 (A*).
- **技术热情**: 专注于高性能、高可用性的纯客户端 Web 应用，追求工程化与极致的用户体验.

## 🛠 技术栈

| 前端 (Frontend) | 后端 & 数据库 (Backend & Database) | 工程化 & DevOps (Tooling & DevOps) |
| :---: | :---: | :---: |
| ![JavaScript](https://img.shields.io/badge/JavaScript-ES202x-F7DF1E?logo=javascript&logoColor=000) | ![C#](https://img.shields.io/badge/C%23-Language-512BD4?logo=c-sharp&logoColor=fff) ![Node.js](https://img.shields.io/badge/Node.js-Backend-43853D?logo=node.js&logoColor=fff) | ![Vite](https://img.shields.io/badge/Vite-Bundler-646CFF?logo=vite&logoColor=fff) |
| ![TypeScript](https://img.shields.io/badge/TypeScript-Types-3178C6?logo=typescript&logoColor=fff) | ![SQL](https://img.shields.io/badge/SQL-Database-4479A1?logo=microsoft-sql-server&logoColor=fff) | ![Nginx](https://img.shields.io/badge/Nginx-Proxy-009639?logo=nginx&logoColor=fff) |
| ![Vue3](https://img.shields.io/badge/Vue-Framework-4FC08D?logo=vue.js&logoColor=fff) ![Nuxt3](https://img.shields.io/badge/Nuxt-Framework-00DC82?logo=nuxt.js&logoColor=fff) | ![Web Workers](https://img.shields.io/badge/Web%20Workers-Parallel-10B981) | ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI/CD-2088FF?logo=githubactions&logoColor=fff) |
| ![Leaflet](https://img.shields.io/badge/Leaflet-2D%20Map-199900?logo=leaflet&logoColor=fff) ![Three.js](https://img.shields.io/badge/Three.js-3D%20Map-000000?logo=three.js&logoColor=fff) ![PixiJS](https://img.shields.io/badge/PixiJS-WebGL-ED4E6E?logo=pixiv&logoColor=fff) ![GSAP](https://img.shields.io/badge/GSAP-Animation-88CE02?logo=greensock&logoColor=fff) | ![数据埋点](https://img.shields.io/badge/Data%20Tracking-Analytics-1E90FF) | ![TailwindCSS](https://img.shields.io/badge/TailwindCSS-Styling-06B6D4?logo=tailwindcss&logoColor=fff) |

**🚀 正在探索 (Currently Exploring):**

![React](https://img.shields.io/badge/React-Library-61DAFB?logo=react&logoColor=000)
![GSAP](https://img.shields.io/badge/GSAP-Animation-88CE02?logo=greensock&logoColor=fff)
![GLSL](https://img.shields.io/badge/GLSL-Shaders-5A86A4?logo=opengl&logoColor=fff)
![GPU](https://img.shields.io/badge/GPU%20Rendering-Performance-BF4040)
![SEO](https://img.shields.io/badge/SEO-Optimization-DE4C36)
![Geo](https://img.shields.io/badge/Geo-Mapping-3399CC)

## ⭐ 精选项目
- 🦀 **RustQuantLab**: 纯客户端高性能永续合约模拟器，无需后端即可在浏览器内完整复刻专业交易所体验。
  - **产品设计**: 深度拆解 Binance/OKX 交易流程，抽象出保证金模型、强平机制、风险分级等核心业务逻辑；UI/UX 对标 TradingView 专业深色主题，注重信息密度与操作效率的平衡。
  - **工程决策**: 选择 Rust→WebAssembly 而非纯 JS，是为了在浏览器内实现毫秒级高频 Tick 处理（1000+ updates/s）同时保证主线程 60fps 渲染不卡顿；通过 serde-wasm-bindgen 零拷贝桥接，消除 JS↔Wasm 数据序列化瓶颈。
  - **前端深度**: React 状态分层架构（引擎层/业务层/视图层解耦）、ECharts 大数据量 K 线渲染优化、CSS Grid 响应式布局（移动端→4K 超宽屏自适应）。
  - *Independently designed Web perpetual contract simulator replicating professional exchange UX. Rust/Wasm engine handles 1000+ ticks/s without blocking UI; React state layering + ECharts optimization; responsive grid layout from mobile to 4K ultrawide.*  
  - Live Demo：https://duri686.github.io/RustQuantLab/  
  - Repo：https://github.com/Duri686/RustQuantLab  
  <img src="https://raw.githubusercontent.com/Duri686/RustQuantLab/refs/heads/main/docs/preview.png" alt="RustQuantLab Preview" width="640" />

- 🗺️ **RoadNetVisualizer**: 纯客户端 3D 室内导航模拟器，完整实现 A* 寻路算法与多楼层路径规划，无后端依赖。
  - **产品设计**: 抽象"楼层-连接点-路径"拓扑模型，支持楼梯/电梯跨层导航（带代价权重）；"点击即导航"零学习成本交互。
  - **工程决策**: 多楼层节点合并统一图，A* 通过 `crossFloor` 边实现跨层寻路；异步执行避免阻塞渲染。
  - **前端深度**: Three.js 3D 场景交互（楼层切换、相机过渡）、路径平滑（视线检测+障碍避让）、实时动画插值。
  - *Pure client-side 3D indoor navigation with A* pathfinding & multi-floor routing. Three.js scene interaction, path smoothing, zero backend dependency.*  
  - Live Demo：https://duri686.github.io/RoadNetVisualizer/  
  - Repo：https://github.com/Duri686/RoadNetVisualizer  
  <img src="https://raw.githubusercontent.com/Duri686/RoadNetVisualizer/refs/heads/main/docs/images/overview.png" alt="Path Preview" width="640" />

## 📊 GitHub 统计
<img src="https://raw.githubusercontent.com/Duri686/Duri686/main/github-stats.svg" alt="GitHub Stats" />

<!-- ## 🏆 Trophies

<p align="left">
  <img src="https://github-trophies.vercel.app/?username=Duri686&theme=flat&column=6&margin-w=8&margin-h=8" alt="trophy" />
</p> -->

## 📈 Activity Graph

[![Duri's Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=Duri686&theme=github-compact&area=true&hide_border=true)](https://github.com/ashutosh00710/github-readme-activity-graph)

## ⭐ Latest Stars
<!-- STARS:START -->

- [clash-verge-rev/clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev) — A modern GUI client based on Tauri, designed to run in Windows, macOS and Linux for tailored proxy experience
- [moonbitlang/moonbit-docs](https://github.com/moonbitlang/moonbit-docs) — The docs of MoonBit programming language
- [zzzgydi/clash-verge](https://github.com/zzzgydi/clash-verge) — A Clash GUI based on tauri. Supports Windows, macOS and Linux.
- [ventoy/Ventoy](https://github.com/ventoy/Ventoy) — A new bootable USB solution.
- [cv-cat/Spider_XHS](https://github.com/cv-cat/Spider_XHS) — 小红书爬虫数据采集，小红书全域运营解决方案
<!-- STARS:END -->

## 📬 Contact
- GitHub Issues (preferred): open an issue in any repo
- Email: <duri@duck.com>
- Website: <https://geo4ai.com/>
- Image Tools: <https://img.geo4ai.com/>
