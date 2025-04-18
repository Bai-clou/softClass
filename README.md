# WhiteHouse.gov Clone Project

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 项目概述
复刻版白宫官方网站，包含新闻发布、政府职能介绍、在线联系等核心功能，采用现代化Web技术栈实现。

## 核心功能

### 功能性需求
- 响应式主页（总统演讲焦点图+快速入口）
- 新闻中心（带分类/时间过滤的新闻系统）
- 政府架构可视化展示（三权分立交互图表）
- 在线联系表单（带文件上传和验证）
- 全文搜索引擎（支持政策文档检索）
- 多语言支持（中英双语切换）
- 管理员后台（基于角色的内容管理系统）

### 非功能性需求
- 军事级安全防护（CSP策略/SQL注入防护）
- AA级无障碍访问（WCAG 2.1标准）
- 亚秒级响应速度（Lighthouse评分90+）
- 跨浏览器兼容（IE11+/现代浏览器）

开发协作
团队成员
Alex Chen (@alexchen-dev)

前端架构设计

交互组件开发

无障碍适配

性能优化

CI/CD流水线搭建

Sam Lee (@samlee-devops)

后端API开发

数据库设计

安全防护实现

搜索引擎集成

云服务部署

协作规范
Git Flow工作流

每日站立会议（北京时间20:00）

代码审查必须通过ESLint+Prettier检查

重要修改需配套单元测试（Jest+React Testing Library）

功能分支命名规范：feat/功能名称 / fix/问题描述

# 快速启动

# 克隆仓库
git clone https://github.com/your-org/whitehouse-clone.git

# 安装依赖
cd frontend && yarn install
cd ../backend && npm install

# 配置环境变量
cp .env.example .env

# 启动开发环境
docker-compose up -d
yarn dev  # 前端
npm run dev  # 后端
## 技术架构

```plaintext
├── 前端（React 18 + TypeScript）
│   ├── 组件库：Material-UI v5
│   ├── 状态管理：Redux Toolkit
│   ├── 路由：React Router 6
│   └── 构建：Vite 4

├── 后端（Node.js 18 + Express）
│   ├── ORM：Prisma 4
│   ├── 数据库：PostgreSQL 14
│   └── 搜索引擎：Elasticsearch 8

├── 基础设施
│   ├── Docker容器化部署
│   ├── Nginx反向代理
│   └── AWS EC2 + S3


