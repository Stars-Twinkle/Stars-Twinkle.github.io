# StarsTwinkle 的小窝

个人主页，纯静态（HTML / CSS / 原生 JavaScript），零依赖、零构建，托管在 GitHub Pages。

线上地址：<https://stars-twinkle.github.io/>

## 文件说明

| 文件 | 用途 |
| --- | --- |
| `index.html` | 整个站点，样式与脚本全部内联在这一个文件里 |
| `avatar.jpg` | 头像 |
| `favicon.png` / `apple-touch-icon.png` | 站点图标 |
| `announcements.json` | 公告数据，页面加载时会读取，所有访客可见 |

## 公告怎么发布

1. 访问 `https://stars-twinkle.github.io/#admin`
2. 输入通行密钥登入
3. 新建 / 修改公告并保存
4. 点「导出 JSON」得到 `announcements.json`
5. 用它覆盖仓库里的 `announcements.json`，提交

> 后台里编辑的内容只保存在**当前浏览器**（localStorage）。要让所有访客看到，必须完成第 4–5 步把它提交到仓库。

## 注意

- 后台入口只是隐藏，通行密钥写在前端源码中，**不具备真正的安全性**，请勿在其中放置敏感信息。
- 更新后页面没变化通常是 GitHub Pages 缓存，等 1–2 分钟或按 Ctrl+F5 强制刷新。

## 本地预览

直接用浏览器打开 `index.html` 即可，不需要服务器。
