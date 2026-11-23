# 参与贡献

感谢你愿意参与 CWFLY。请先读完本文，再开始动手。

## 先看这些

- 官网：<https://www.cwflysim.cn>
- 文档：<https://docs.cwflysim.cn>
- 各仓库的 `README.md` 有该项目的运行方式与目录说明

## 提交问题

- 在**对应的仓库**提 Issue，不要跨仓库乱发
- 提供可复现的信息：环境、版本、复现步骤、期望结果与实际结果；界面问题请附截图
- 安全漏洞**不要**提 Issue，按 [SECURITY.md](SECURITY.md) 走加密邮件

## 提交代码

1. Fork 目标仓库，从 `main` 切出功能分支（如 `feat/online-map-clustering`、`fix/login-redirect`）
2. 保持与现有代码风格一致，不做与议题无关的格式化改动
3. 本地自测通过，涉及接口/配置的改动请同步更新文档
4. 提 Pull Request 到 `main`，描述里写清：
   - 改动动机与关联 Issue
   - 具体改了什么、影响范围
   - 如何验证（命令、截图或录屏）

## 代码约定（摘要）

- 后端：Python 3.11+，FastAPI + SQLAlchemy 2.0；接口返回统一 `{success, data}` / `{success:false, code, message}`
- 前端：Vue 3 `<script setup>` + Pinia，样式优先使用项目已有的 CSS 变量与设计令牌，避免写死颜色
- 提交信息：`type(scope): subject`，type 取 `feat|fix|refactor|docs|chore|style|perf|test`

## 许可

向本组织提交贡献即表示你同意该贡献以目标仓库的许可证（默认为 GPL-3.0）发布。
