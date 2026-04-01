# OKX下载指南网站 - 深色高级版

一个现代、专业的静态网站,采用深色主题设计,类似OKX官方风格,提供OKX官方客户端下载链接和邀请码展示。

## 功能特点

- ✅ **深色高级主题**:采用OKX风格的深色设计,霓虹蓝渐变,玻璃态效果
- ✅ 响应式设计,适配手机和电脑
- ✅ 官方原版OKX客户端下载(Windows/iOS/Android)
- ✅ 邀请码展示和复制功能(带发光效果)
- ✅ 清晰的使用指南步骤
- ✅ 安全警告和免责声明
- ✅ 现代美观的UI设计,带悬浮动画和渐变效果
- ✅ 玻璃态设计(Glassmorphism)和毛玻璃效果
- ✅ 平滑动画和过渡效果

## 快速部署

### 方法一:GitHub Pages(推荐)

1. 在GitHub上创建新仓库
2. 上传本文件夹所有文件到仓库
3. 进入仓库设置 → Pages
4. 选择分支(通常是main/master)和根目录
5. 保存后等待部署完成(约1分钟)
6. 访问 `https://你的用户名.github.io/仓库名/`

### 方法二:直接上传到你的服务器

1. 将 `index.html`, `style.css` 等文件上传到你的网站根目录
2. 确保域名 `okx-zhinan.com` 已解析到服务器
3. 访问 `https://okx-zhinan.com` 查看效果

### 方法三:本地预览

1. 双击 `index.html` 用浏览器打开
2. 或使用本地服务器:
   ```bash
   # Python 3
   python -m http.server 8000

   # 然后访问 http://localhost:8000
   ```

## 配置你的邀请链接和邀请码

网站已配置为包含：
1. **直接注册按钮**：链接到 `https://www.promoohubly.com/join/9045338`
2. **邀请码显示**：9045338（带发光效果和复制功能）

如需修改：

### 步骤1：获取你的OKX邀请链接或邀请码

1. 登录OKX节点后台
2. 获取你的专属邀请链接（如 `https://www.promoohubly.com/join/你的邀请码`）
3. 或获取邀请码（通常是6-8位字母数字组合）

### 步骤2：替换邀请链接

打开 `index.html` 文件，搜索以下内容：
```html
<a href="https://www.promoohubly.com/join/9045338" class="register-btn" target="_blank">
```

将 `https://www.promoohubly.com/join/9045338` 替换为你的新邀请链接。

### 步骤3：替换邀请码

在同一文件中搜索：
```javascript
const inviteCode = '9045338';
```

将 `'9045338'` 替换为你的新邀请码。

### 步骤4：测试功能

1. 刷新网页，直接注册按钮应正常显示（绿-蓝渐变）
2. 点击"立即注册 OKX"按钮测试链接跳转
3. 邀请码应正常显示（带霓虹蓝发光效果）
4. 点击"复制邀请码"按钮测试复制功能

## 自定义修改

### 修改网站标题
在 `index.html` 第7行修改 `<title>` 标签内容。

### 修改配色方案(深色主题)
在 `style.css` 文件的 `:root` 部分修改颜色变量:
- `--primary-color`: 主背景色(#0a0e17)
- `--secondary-color`: 次要背景色(#121826)
- `--accent-color`: 强调色(霓虹蓝 #00d4ff)
- `--accent-gradient`: 渐变强调色(linear-gradient(90deg, #00d4ff, #0095ff))
- `--text-primary`: 主要文字颜色(#ffffff)
- `--text-secondary`: 次要文字颜色(#b0b7c3)
- `--card-bg`: 卡片背景(rgba(18, 24, 38, 0.8))

### 更新下载链接
如果需要更新官方下载链接,修改 `index.html` 中的下载按钮链接:
- Windows下载链接(搜索"Windows下载按钮")
- iOS App Store链接(搜索"前往App Store")
- Android Google Play链接(搜索"前往Google Play")

## 重要警告

⚠️ **域名风险提示**
OKX节点计划规则禁止使用与官方相似的域名(如 `okx-xxx.com`)。你的域名 `okx-zhinan.com` 可能被判定为相似域名,**有节点资格被取消的风险**。

建议:
1. 考虑更换域名(如 `crypto-zhinan.com`)
2. 或在网站显著位置添加免责声明(已内置)
3. 不要以OKX官方名义宣传

## 网站结构

```
okx-download-site/
├── index.html          # 主页面
├── style.css          # 样式文件
├── README.md          # 说明文件
└── (未来可添加)
    ├── favicon.ico    # 网站图标
    ├── images/        # 图片资源
    └── js/           # 额外JavaScript
```

## SEO优化建议

1. 在 `<meta name="description">` 中添加详细描述
2. 考虑添加Google Analytics跟踪代码
3. 提交网站到百度站长平台和Google Search Console
4. 创建网站图标(favicon)

## 技术支持

如有问题:
1. 检查浏览器控制台是否有错误(F12 → Console)
2. 确保邀请码已正确替换
3. 确保所有文件在同一目录

## 法律声明

本网站模板仅供个人学习使用。实际部署时请遵守当地法律法规和OKX平台规则。开发者不承担因使用本模板产生的任何责任。

---

**最后更新:2024年4月**