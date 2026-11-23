<div align="center">

# CWFLY · 青翼模拟飞行

**面向模拟飞行爱好者的连飞平台** —— 社区站点、FSD 连线服务器、ATC 管制工作台、QQ 机器人与文档站

[![官网](https://img.shields.io/badge/官网-www.cwflysim.cn-0b6cf0?style=flat-square)](https://www.cwflysim.cn)
[![ATC](https://img.shields.io/badge/ATC-atc.cwflysim.cn-0b6cf0?style=flat-square)](https://atc.cwflysim.cn)
[![文档](https://img.shields.io/badge/文档-docs.cwflysim.cn-0b6cf0?style=flat-square)](https://docs.cwflysim.cn)
[![安全披露](https://img.shields.io/badge/安全披露-PGP-2ea043?style=flat-square)](https://www.cwflysim.cn/security)
[![License](https://img.shields.io/badge/license-GPL--3.0-6e7781?style=flat-square)](https://www.gnu.org/licenses/gpl-3.0.html)

</div>

---

## 关于

CWFLY（CyanWing Flight Simulation Platform，青翼模拟飞行平台）是一套自建的模拟飞行连飞基础设施，用于替代第三方连飞网络，把「连飞」「管制」「社区」放在同一个账号体系下：

- 一个 CWFLY 账号即可登录社区站点、ATC 工作台与所有内部服务（OAuth2 授权码 + PKCE，支持 Passkey / WebAuthn）
- 自研 FSD 连线服务器承载机长与管制的实时会话，支持广播裁剪、会话重连、飞行计划锁定
- 社区站点提供在线地图、航图、气象、飞行计划、培训与论坛
- 文档站收录新人指南、管制手册与 FSD 使用说明

平台位于中国，面向中文模拟飞行社区，**仅供模拟飞行娱乐使用，与真实航空运行无关**。

## 项目

| 仓库 | 说明 | 主要技术 |
| --- | --- | --- |
| [CWFLY-WEB](https://github.com/CyanWing-Flight-Simulation-Platform/CWFLY-WEB) | 社区站点与后端 API：账号体系、在线地图、航图、气象、飞行计划、培训、论坛、第三方 OAuth2 授权服务 | FastAPI · SQLAlchemy · Vue 3 · MySQL |
| [CWFLY-FSD](https://github.com/CyanWing-Flight-Simulation-Platform/CWFLY-FSD) | FSD 连线服务器：认证、广播裁剪、会话重连、飞行计划锁定、METAR 多源聚合 | Python asyncio |
| [CWFLY-ATC](https://github.com/CyanWing-Flight-Simulation-Platform/CWFLY-ATC) | ATC 管制中心：席位工作台、在线管制、雷达边界、排班与交接 | Vue |
| [CWFLY-BOT](https://github.com/CyanWing-Flight-Simulation-Platform/CWFLY-BOT) | QQ 机器人：群管理、航班查询、FSD 状态播报、AI 问答 | Python · OneBot v11 |
| [CWFLY-DOCS](https://github.com/CyanWing-Flight-Simulation-Platform/CWFLY-DOCS) | 官方文档站：新人指南、管制手册、FSD 使用说明、API 文档 | VitePress |

## 技术栈

`Python` · `FastAPI` · `SQLAlchemy 2.0` · `MySQL 8` · `Vue 3` · `Pinia` · `Vite` · `WebSocket` · `WebAuthn` · `OAuth 2.0 / PKCE` · `PM2` · `Nginx`

## 参与

- **问题与建议**：在对应仓库提 Issue；提问前先看 [文档站](https://docs.cwflysim.cn)
- **代码贡献**：欢迎 Pull Request，请保持与现有代码风格一致，并在描述里写清改动动机与影响范围
- **安全漏洞**：请**不要**在公开 Issue 中披露未修复的漏洞，按 [安全漏洞披露政策](https://www.cwflysim.cn/security) 通过加密邮件报告；公钥与 `security.txt` 见 `cwflysim.cn/.well-known/`

## 联系

- 官网：<https://www.cwflysim.cn>
- 文档：<https://docs.cwflysim.cn>
- 加入 QQ 群：<https://qm.qq.com/q/yvXQbE1Sym>
- 邮箱：support@cwflysim.cn

## 许可

各仓库除特别说明外均采用 [GPL-3.0](https://www.gnu.org/licenses/gpl-3.0.html) 许可。CWFLY 与波音、空客及任何真实航空公司、民航管理机构无关。
