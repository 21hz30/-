# 值日管理系统

一个用于管理和追踪值日考勤情况的 Web 应用。

## 功能特点

- 📅 值日排班表显示
- 👥 8个值日组（每组3人）管理
- ✅ 考勤状态记录（已到/迟到/缺席）
- 📊 考核评分系统
- 🔍 详细的统计分析
- 👮‍♂️ 管理员权限控制

## 技术栈

- React 18
- Next.js 14
- TypeScript
- TailwindCSS
- date-fns

## 安装步骤

1. 克隆项目
bash
git clone [项目地址]
cd [项目目录]

2. 安装依赖

bash
npm install

3. 运行开发服务器

bash
npm run dev

4. 打开浏览器访问 http://localhost:3000

## 项目依赖

```json
{
  "dependencies": {
    "next": "14.1.0",
    "react": "^18",
    "react-dom": "^18",
    "date-fns": "^3.0.0"
  },
  "devDependencies": {
    "@types/node": "^20",
    "@types/react": "^18",
    "@types/react-dom": "^18",
    "autoprefixer": "^10.0.1",
    "postcss": "^8",
    "tailwindcss": "^3.3.0",
    "typescript": "^5"
  }
}
```

## 项目结构

```
src/
├── components/          # 组件目录
│   ├── AttendanceModal.tsx    # 考勤评分弹窗
│   ├── LoginModal.tsx         # 登录弹窗
│   └── RecordDetailModal.tsx  # 记录详情弹窗
├── config/             # 配置文件
│   └── admin.ts       # 管理员账号配置
├── data/              # 数据文件
│   └── groups.ts      # 值日组数据
├── pages/             # 页面文件
│   ├── index.tsx      # 首页（排班表）
│   └── statistics.tsx # 统计页面
├── styles/            # 样式文件
│   └── globals.css    # 全局样式
└── types/             # 类型定义
    └── index.ts       # 类型声明文件
```

## 管理员账号

- 用户名：admin1 或 admin2
- 密码：admin123

## 功能说明

1. 值日排班表
   - 显示每周值日组安排
   - 查看每天值日人员
   - 记录考勤状态

2. 考核评分
   - 记录出勤状态
   - 评分系统（1-10分）
   - 惩罚值日天数设置
   - 备注信息

3. 统计分析
   - 按组别筛选
   - 查看平均分
   - 出勤统计
   - 惩罚天数统计
   - 详细记录查看

## 使用的颜色

- 蓝色（主题色）：#2a63b7
- 红色（警告色）：#ff2300
- 绿色（成功色）：#00bd39

## 浏览器支持

- Chrome (推荐)
- Firefox
- Safari
- Edge

## 注意事项

- 数据存储使用 localStorage，刷新页面数据不会丢失
- 需要管理员权限才能进行考勤评分
- 所有用户都可以查看排班和统计信息

## 开发环境要求

- Node.js 18.0.0 或更高版本
- npm 9.0.0 或更高版本



