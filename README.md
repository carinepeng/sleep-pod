# 午休舱预订系统

## 文件说明
- `index.html` — 用户预订页
- `admin.html` — 管理后台
- `vercel.json` — Vercel 部署配置

## 部署步骤

### 第一步：上传到 GitHub
1. 打开 https://github.com，登录
2. 点右上角 + → New repository
3. 名字填 `sleep-pod`，选 Public，点 Create
4. 点 uploading an existing file
5. 把 index.html、admin.html、vercel.json 三个文件拖进去
6. 点 Commit changes

### 第二步：部署到 Vercel
1. 打开 https://vercel.com，用 GitHub 账号登录
2. 点 Add New Project
3. 选刚才创建的 sleep-pod 仓库
4. 直接点 Deploy（不用改任何设置）
5. 等约1分钟，完成后会给你一个网址，如 https://sleep-pod-xxx.vercel.app

### 第三步：配置收款码
1. 把收款码图片上传到任意图床（如 https://imgbb.com）
2. 复制图片链接
3. 打开 index.html，找到这行：
   const QR_CODE_URL = 'YOUR_QR_CODE_IMAGE_URL';
4. 替换为真实图片链接
5. 重新上传到 GitHub，Vercel 自动更新

### 访问地址
- 用户预订页：https://你的域名.vercel.app/
- 管理后台：https://你的域名.vercel.app/admin

### 默认管理员密码
用户名：admin
密码：admin123

修改密码：打开 admin.html，找到：
const ADMIN_PASSWORD = 'admin123';
改成你想要的密码，重新上传即可。
