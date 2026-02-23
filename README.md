<div align="center">
  <img width="120" height="120" alt="logo" src="https://github.com/user-attachments/assets/f31979aa-48d3-4789-93a0-d45db1f99568" />

  <h1 style="font-family: 'Microsoft YaHei', 'PingFang SC', 'Hiragino Sans GB', sans-serif; font-size: 2.5rem; font-weight: bold; color: #B22222; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);">泡泡</h1>
  <p>人生处处有故事</p>
  <p>
    <a href="https://www.powpow.online/">https://www.powpow.online/</a>
  </p>
  🚧 当前状态：项目积极开发中 (Work in Progress)
  <p>
    <img src="https://img.shields.io/badge/Next.js-16.1.1-blue?style=flat-square" alt="Next.js" />
    <img src="https://img.shields.io/badge/React-19.2.3-blue?style=flat-square" alt="React" />
    <img src="https://img.shields.io/badge/TypeScript-5-blue?style=flat-square" alt="TypeScript" />
    <img src="https://img.shields.io/badge/Tailwind%20CSS-4-blue?style=flat-square" alt="Tailwind CSS" />
    <img src="https://img.shields.io/badge/PostgreSQL-15-blue?style=flat-square" alt="PostgreSQL" />
    <img src="https://img.shields.io/badge/Leaflet-1.9.4-green?style=flat-square" alt="Leaflet" />
    <img src="https://img.shields.io/badge/OpenClaw-Integrated-purple?style=flat-square" alt="OpenClaw Integration" />
    <img src="https://img.shields.io/badge/WebSocket-8.16.0-orange?style=flat-square" alt="WebSocket" />
  </p>
</div>
  
## 📱 应用界面

<table>
  <tr>
    <td style="text-align: center;"><img src="https://github.com/user-attachments/assets/7042bc62-adb6-41fe-8710-619b53f2b31d" width="200" /><br/><sub>泡泡地图界面</sub></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td style="text-align: center;"><img src="https://github.com/user-attachments/assets/1eba2c2a-07a5-4416-a4fb-e0608d79dd18" width="200" /><br/><sub>数字人对话界面</sub></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td style="text-align: center;"><img src="https://github.com/user-attachments/assets/6e85ea85-dc34-4f3d-8737-657aaeee9303" width="200" /><br/><sub>发布泡泡界面</sub></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td style="text-align: center;"><img src="https://github.com/user-attachments/assets/f1498bcc-681e-4bcb-bea1-b895311ce645" width="200" /><br/><sub>社交互动界面</sub></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td style="text-align: center;"><img src="https://github.com/user-attachments/assets/2f3ca982-4c85-4b75-a4a6-cdfe44d17621" width="200" /><br/><sub>个人中心界面</sub></td>
  </tr>
</table>

## 📖 项目介绍

**泡泡**是一个基于地理位置的社交应用，致力于记录和分享生活中的精彩故事。无论你在哪里，都可以通过泡泡发布带有位置信息的内容，与附近的人分享你的生活点滴，发现身边的精彩故事。

### 项目理念
"人生处处有故事"是泡泡的核心理念。我们相信每个人的生活中都有值得记录和分享的瞬间，每个地方都有独特的故事等待被发现。通过泡泡，你可以：

- 在特定地点留下你的故事和回忆
- 发现身边其他人分享的精彩内容
- 与附近的数字人互动，了解当地的文化和历史
- 建立基于地理位置的社交连接

### 项目亮点
- **地理位置社交**：基于地图的内容浏览和发布，探索身边的故事
- **数字人互动**：与特定地点的数字人对话，获得个性化的本地信息
- **多媒体内容**：支持图片、音频、音乐等多种形式的内容发布
- **社交分享**：轻松分享你的故事到社交平台，与更多人分享精彩
- **智能推荐**：根据你的位置和兴趣，推荐相关的内容和数字人

### 技术特色
- 使用 Next.js 16.1.1 构建，支持 SSR 和 SSG，提供优秀的性能和 SEO
- 采用 React 19.2.3 + TypeScript 确保类型安全和代码质量
- 使用 Tailwind CSS 4 实现响应式设计，适配各种设备
- PostgreSQL 数据库存储用户数据和内容
- Leaflet 地图库实现地理位置功能，提供流畅的地图体验
- 集成人工智能技术，实现数字人对话功能
- **OpenClaw 集成**：支持通过 OpenClaw 技能控制地图上的机器人
- **WebSocket 实时通信**：实现机器人状态实时更新和控制

## 🤖 OpenClaw 集成

### 功能介绍
泡泡现已集成 OpenClaw 机器人控制功能，通过 OpenClaw 技能可以：

- **发送机器人到地图**：在指定位置创建机器人实体
- **控制机器人移动**：实时控制机器人在地图上的位置
- **执行任务**：发送巡逻、问候、送达、探索等任务
- **实时监控**：通过 WebSocket 实时获取机器人状态
- **与用户交互**：机器人可以与地图上的用户进行互动

### OpenClaw 技能

#### bubble-robot 技能
- **位置**：`skills/openclaw-bubble-robot/`
- **功能**：控制泡泡地图上的机器人
- **API**：提供完整的机器人管理和控制接口

#### 技能使用示例

```javascript
const BubbleRobotSkill = require('./skills/openclaw-bubble-robot');

// 创建技能实例
const robotSkill = new BubbleRobotSkill({
  apiBase: 'http://localhost:3000/api/openclaw'
});

// 创建机器人
const robot = await robotSkill.createRobot(
  '巡逻机器人',
  { lat: 39.9042, lng: 116.4074 },
  '用于地图巡逻的 OpenClaw 机器人'
);

// 移动机器人
await robotSkill.moveRobot(
  robot.id,
  { lat: 39.9142, lng: 116.4174 },
  'patrol'
);

// 发送任务
await robotSkill.sendTask(
  robot.id,
  'greet',
  { lat: 39.9242, lng: 116.4274 },
  'user123'
);
```

### API 接口

#### 机器人管理
- `POST /api/openclaw/robots`：创建新机器人
- `GET /api/openclaw/robots`：获取机器人列表
- `GET /api/openclaw/robots/:id`：获取机器人详情
- `PUT /api/openclaw/robots/:id`：更新机器人状态
- `DELETE /api/openclaw/robots/:id`：删除机器人

#### WebSocket 服务
- **地址**：`ws://localhost:8080`
- **功能**：实时推送机器人状态更新
- **消息类型**：`robot_created`、`robot_moved`、`robot_status_updated` 等

### 控制面板

项目包含 `OpenClawRobotControl` 组件，提供：

- 机器人列表展示
- 创建新机器人
- 发送任务控制
- 监控机器人状态
- 删除机器人

### 部署指南

#### 1. 安装依赖
```bash
pnpm install
```

#### 2. 数据库迁移
```bash
node src/storage/database/migrate-openclaw-robots.ts
```

#### 3. 启动服务
```bash
pnpm dev
```

#### 4. 部署 OpenClaw 技能
1. **打包技能**：
   ```bash
   cd skills/openclaw-bubble-robot
   zip -r bubble-robot.zip .
   ```

2. **发布到 ClawdHub**：
   - 登录 ClawdHub
   - 上传 `bubble-robot.zip`
   - 配置 API 密钥

### 技术架构

```
┌─────────────┐     ┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│             │     │              │     │              │     │              │
│  OpenClaw   │────>│  OpenClaw    │────>│  后端 API    │────>│  地图系统    │
│  客户端     │     │  机器人技能   │     │  (Robots API) │     │  (Map + DB)   │
│             │     │              │     │              │     │              │
└─────────────┘     └──────────────┘     └──────────────┘     └──────────────┘
        ^                     ^                     ^                     ^
        │                     │                     │                     │
        └─────────────────────┼─────────────────────┼─────────────────────┘
                              │                     │
                              └─────────────────────┘
                               WebSocket 实时通信
```

## 🚀 快速开始

### 环境要求
- Node.js 18.0 或更高版本
- pnpm 9.0.0 或更高版本
- PostgreSQL 14.0 或更高版本

### 安装步骤

1. **克隆仓库**
   ```bash
   git clone https://github.com/durenzidu/powpow.git
   cd powpow
   ```

2. **安装依赖**
   ```bash
   pnpm install
   ```

3. **配置环境变量**
   ```bash
   # 复制环境配置文件
   cp .env.example .env
   
   # 编辑 .env 文件，填写相应的配置
   # 可以使用文本编辑器打开并修改
   ```

4. **启动开发服务器**
   ```bash
   pnpm run dev
   ```
   访问 http://localhost:3000 查看项目

5. **构建生产版本**
   ```bash
   pnpm run build
   ```

6. **启动生产服务**
   ```bash
   pnpm start
   ```

## 📁 项目结构

```
powpow/
├── src/
│   ├── app/             # Next.js 应用路由
│   │   ├── act1/         # 第一幕剧情
│   │   ├── act2/         # 第二幕剧情
│   │   ├── act3/         # 第三幕剧情
│   │   ├── act4/         # 第四幕剧情
│   │   ├── act5/         # 第五幕剧情
│   │   ├── api/          # API 路由
│   │   ├── admin/        # 管理员系统
│   │   ├── digital-humans/ # 数字人相关页面
│   │   ├── map/          # 地图页面
│   │   ├── posts/         # 内容详情页面
│   │   ├── profile/       # 用户 profile 页面
│   │   ├── publish/       # 发布内容页面
│   │   └── page.tsx       # 首页
│   ├── components/       # 组件库
│   │   ├── ui/           # 通用 UI 组件
│   │   ├── editor/       # 编辑器组件
│   │   ├── DigitalHumanChat.tsx # 数字人聊天组件
│   │   ├── LeftBottomMenu.tsx # 底部菜单组件
│   │   ├── LocationPicker.tsx # 位置选择组件
│   │   ├── MapComponent.tsx # 地图组件
│   │   ├── PostContentRenderer.tsx # 内容渲染组件
│   │   └── ...           # 其他组件
│   ├── lib/              # 工具函数和服务
│   │   ├── services/     # 外部服务
│   │   ├── utils/        # 通用工具
│   │   ├── auth.ts       # 认证相关
│   │   ├── geocode.ts     # 地理编码
│   │   ├── location.ts    # 位置相关
│   │   └── ...           # 其他工具
│   ├── storage/          # 数据库相关代码
│   │   ├── database/     # 数据库管理
│   │   └── ...           # 其他存储
│   ├── types/            # TypeScript 类型定义
│   ├── contexts/         # React 上下文
│   │   ├── AuthContext.tsx # 认证上下文
│   │   ├── AudioContext.tsx # 音频上下文
│   │   └── ...           # 其他上下文
│   ├── hooks/            # 自定义 Hooks
│   │   ├── useLocation.ts # 位置相关 Hook
│   │   ├── useCheckIns.ts # 打卡相关 Hook
│   │   └── ...           # 其他 Hooks
│   └── middleware.ts     # 中间件
├── public/               # 静态资源
│   ├── assets/           # 图片等资源
│   ├── favicon.png       # 网站图标
│   └── logo.png          # 网站 Logo
├── scripts/              # 脚本文件
├── .env.example          # 环境变量示例
├── package.json          # 项目配置
├── tsconfig.json         # TypeScript 配置
└── README.md             # 项目说明
```

## ✨ 功能特性

### 1. 地图社交
- **地图浏览**：在地图上查看附近的泡泡内容
- **位置标记**：在特定地点发布内容，留下你的故事
- **距离显示**：显示内容发布地点与你的距离
- **位置搜索**：搜索特定地点的泡泡内容

### 2. 数字人互动
- **附近数字人**：发现身边的数字人
- **实时对话**：与数字人进行实时聊天
- **个性化互动**：每个数字人都有独特的性格和背景
- **本地信息**：数字人可以提供当地的文化、历史和旅游信息

### 3. 内容发布
- **多媒体支持**：发布图片、音频、音乐等多种形式的内容
- **位置选择**：选择内容发布的具体位置
- **富文本编辑**：支持文本格式化、表情等
- **内容预览**：发布前预览内容效果

### 4. 社交互动
- **点赞评论**：对泡泡内容进行点赞和评论
- **分享功能**：分享泡泡内容到其他社交平台
- **关注用户**：关注感兴趣的用户，查看他们的动态
- **消息通知**：接收评论、点赞和关注通知

### 5. 个人中心
- **个人资料**：编辑个人信息和头像
- **我的泡泡**：查看自己发布的所有内容
- **我的收藏**：查看收藏的内容
- **我的关注**：查看关注的用户

### 6. 管理员系统
- **内容管理**：管理用户发布的内容
- **用户管理**：管理用户账号和权限
- **数字人管理**：创建和管理数字人
- **数据统计**：查看应用使用数据和用户行为

## 🛠️ 部署指南

### 选项 1：使用 Vercel 部署（推荐）

1. **连接 GitHub 仓库**
   - 登录 Vercel 账号
   - 点击 "New Project"
   - 选择 powpow 仓库

2. **配置环境变量**
   - 在 Vercel 项目设置中，添加 `.env` 文件中的环境变量

3. **部署项目**
   - 点击 "Deploy" 按钮
   - Vercel 会自动构建和部署项目

4. **配置域名**
   - 在 Vercel 项目设置中，添加自定义域名 `www.powpow.online`

### 选项 2：使用 Docker 容器化部署

1. **创建 Dockerfile**
   ```dockerfile
   FROM node:18-alpine
   
   WORKDIR /app
   
   COPY package*.json ./
   RUN npm install -g pnpm
   RUN pnpm install
   
   COPY . .
   
   RUN pnpm run build
   
   EXPOSE 3000
   
   CMD ["pnpm", "start"]
   ```

2. **构建镜像**
   ```bash
   docker build -t powpow .
   ```

3. **运行容器**
   ```bash
   docker run -d -p 3000:3000 --env-file .env powpow
   ```

### 选项 3：使用传统服务器部署

1. **准备服务器**
   - 安装 Node.js 18.0+ 和 PostgreSQL 14.0+
   - 配置防火墙，开放 3000 端口
   - 配置域名 `www.powpow.online` 指向服务器 IP

2. **部署代码**
   - 克隆仓库到服务器
   - 安装依赖
   - 构建项目

3. **启动服务**
   - 使用 PM2 管理进程
   ```bash
   npm install -g pm2
   pm2 start "pnpm start" --name powpow
   pm2 save
   pm2 startup
   ```

4. **配置 Nginx 反向代理**
   ```nginx
   server {
     listen 80;
     server_name www.powpow.online powpow.online;
     
     location / {
       proxy_pass http://localhost:3000;
       proxy_http_version 1.1;
       proxy_set_header Upgrade $http_upgrade;
       proxy_set_header Connection 'upgrade';
       proxy_set_header Host $host;
       proxy_set_header X-Real-IP $remote_addr;
       proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
       proxy_set_header X-Forwarded-Proto $scheme;
       proxy_cache_bypass $http_upgrade;
     }
   }
   ```

5. **配置 SSL 证书**
   - 使用 Let's Encrypt 获取免费 SSL 证书
   - 配置 HTTPS 访问

## 🤝 贡献指南

欢迎贡献代码和提出建议！请按照以下步骤进行：

1. **Fork 仓库**
2. **创建分支**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **提交更改**
   ```bash
   git commit -m "Add your feature"
   ```
4. **推送分支**
   ```bash
   git push origin feature/your-feature-name
   ```
5. **创建 Pull Request**

### 代码规范
- 使用 TypeScript 编写代码
- 遵循 ESLint 规则
- 提交消息使用语义化格式
- 为新功能添加测试
- 保持代码风格一致

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 📞 联系方式

- **项目维护者**：[durenzidu](https://github.com/durenzidu)
- **官方网站**：[https://www.powpow.online/](https://www.powpow.online/)
- **GitHub**：[https://github.com/durenzidu/powpow](https://github.com/durenzidu/powpow)
- **邮箱**：[dongtao@outlook.com](mailto:dongtao@outlook.com)

## 🙏 致谢

感谢所有为项目做出贡献的开发者和支持者！

- 感谢 Next.js 团队提供优秀的框架
- 感谢 React 团队的持续创新
- 感谢 Tailwind CSS 团队的优秀设计工具
- 感谢 Leaflet 团队提供的地图库
- 感谢所有测试和使用本项目的用户

---

<div align="center">
  <p>✨ 泡泡 - 人生处处有故事 ✨</p>
  <p><a href="https://www.powpow.online/" target="_blank" style="color: #B22222; text-decoration: none;">https://www.powpow.online/</a></p>
  <p>© 2026 泡泡团队. All rights reserved.</p>
</div>
