# AI 准备就绪学校推广行动

一个面向中国教育领域的 **AI 就绪学校推广平台**，通过交互式地图与可视化界面，展示在 AI 教育方面表现突出的学校，并传达组织章程与推广理念。

## 功能特性

- **交互式中国地图**：以散点 + 涟漪动效展示各地优秀学校位置，支持缩放与拖拽
- **明/暗双主题**：默认深色科技风格，支持一键切换亮色主题
- **学校名录侧边栏**：可折叠列表，点击条目可联动地图高亮定位
- **组织章程展示**：手风琴式折叠面板，涵盖组织总则、使命、架构、财务等 8 章内容
- **响应式布局**：兼容桌面端与移动端

## 技术栈

| 类型 | 技术 |
|------|------|
| 前端 | HTML5 + Vanilla JavaScript + CSS3 |
| 数据可视化 | [ECharts 5.4.3](https://echarts.apache.org/) |
| 地图数据 | 中国行政区划 GeoJSON |
| 部署方式 | 静态文件，无需构建 |

## 文件结构

```
ai_ready_school/
├── index.html     # 主应用页面（含 HTML / CSS / JS）
├── charter.js     # 组织章程数据（8 章）
├── china.js       # 中国地图 GeoJSON 数据（JS 格式）
├── china.json     # 中国地图 GeoJSON 数据（JSON 格式）
└── favicon.png    # 网站图标
```

## 快速开始

该项目为纯静态应用，无需安装依赖或执行构建，只需通过任意 HTTP 服务器托管文件即可。

**方式一：使用 Python 本地服务**

```bash
# Python 3
python -m http.server 8080
```

然后访问 [http://localhost:8080](http://localhost:8080)

**方式二：使用 VS Code Live Server 插件**

安装 [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) 插件后，右键 `index.html` 选择 `Open with Live Server`。

**方式三：部署至 GitHub Pages**

将仓库推送至 GitHub 后，在仓库设置中开启 GitHub Pages，选择对应分支即可在线访问。

## 组织章程简介

本平台所推广的"AI 准备就绪学校"倡议是一个非营利性公益组织，核心使命包括：

- AI 教育普及与推广
- 教育资源共享
- 教师 AI 能力培训
- 优秀经验传播

组织坚持教育公平、技术伦理与教育诚信原则，面向学校、教育工作者及相关机构开放加入。

## 许可证

本项目内容版权归原作者所有，仅供学习与展示使用。
