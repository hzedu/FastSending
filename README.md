<h1 align="center">FastSend 文件快传 🚀</h1>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/version-0.6.0-blue.svg?style=flat-square" />
  <a href="#" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square" />
  </a>
</p>

<p align="center">
  <img src="./public/ogImg.webp" />
</p>

## 📖 项目介绍

FastSend 是一个基于 WebRTC 技术的点对点文件传输工具，支持快速的目录同步和文件传输。通过浏览器即可实现安全、高效的文件共享。

🌐 在线体验：[fastsend.ing](https://fastsend.ing)

基于原项目添加了共享文本的功能，由于代码风格太差，故不推送仅自己使用，需要可取
![image](https://github.com/user-attachments/assets/ae5e4d8f-2a20-4d1a-9ad6-3ccc8f914cb6)
![image](https://github.com/user-attachments/assets/d999fcd7-593c-42c0-8f22-4dc1e800f977)
![image](https://github.com/user-attachments/assets/d1c130d7-3443-4c4c-9423-a8589de58861)
![image](https://github.com/user-attachments/assets/2509e08b-dbcf-4e3d-89a7-e036d581ef18)

## ✨ 特性

- 🔒 点对点加密传输，确保数据安全
- 📁 支持文件和文件夹传输
- 🚀 局域网自动优化，传输更快
- 🎯 简单易用的界面设计
- 🌍 支持中英文界面
- 📲 支持PWA轻量安装

## 🛠️ 技术栈

- WebRTC
- Vue.js
- Nuxt3
- TypeScript
- Modern File System API

## 📦 安装与构建

```bash
# 安装依赖
yarn install

# 构建项目
yarn build
```

## 🚀 使用方法

```bash
# 启动服务
node .output/server/index.mjs
```

> [!IMPORTANT]
> 目录传输和同步需要 `HTTPS` 以及浏览器支持，一般新版本的桌面浏览器都支持
> 
> 本项目自身的 HTTPS 配置方式（测试环境）请参考：
> 
> - [置顶 Issue](https://github.com/ShouChenICU/FastSend/issues/9#issuecomment-2562353775)
> - [Nuxt 部署教程（英文）](https://nuxt.com/docs/4.x/getting-started/deployment#entry-point)
> 
> FastSend 不建议直接以 HTTPS 形式进行生产环境部署，而应当位于反向代理服务器之后，请参考：
> 
> - [Nginx](https://nginx.org/en/docs/http/configuring_https_servers.html)
> - [Apache httpd](https://httpd.apache.org/docs/current/ssl/)
> - [Caddy](https://caddyserver.com/docs/quick-starts/https)
> - [Windows IIS](https://learn.microsoft.com/zh-cn/iis/manage/configuring-security/how-to-set-up-ssl-on-iis)

## 🐳 Docker 和 Docker Compose

### Docker 构建

```bash
docker build -t fastsend .
docker run -d --name fastsend -p 3000:3000 fastsend
```

### Docker Compose

将项目拉取到本地，然后运行：

```bash
docker-compose up -d
```

访问 `http://localhost:3000` 即可使用。

## 💡 使用提示

1. 确保浏览器启用了 WebRTC 功能
2. 如需传输文件夹或同步目录，请确保浏览器支持现代文件系统 API 并已启用 HTTPS 传输
3. 在同一局域网内传输速度最快
4. 建议在网络状态良好时使用，部分网络环境可能会阻止 P2P / WebRTC 正确建立连接，从而导致传输失败

## 👨‍💻 作者

**ShouChen**

- 博客: [shouchen.blog](https://shouchen.blog)
- X: [@ShouChen\_](https://x.com/ShouChen_)

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📝 开源协议

本项目基于 MIT 协议开源。

## ⭐ 支持项目

如果这个项目对你有帮助，欢迎给一个 star 支持一下！

---

<a href="https://star-history.com/#ShouChenICU/Fastsend&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=ShouChenICU/Fastsend&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=ShouChenICU/Fastsend&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=ShouChenICU/Fastsend&type=Date" />
 </picture>
</a>
