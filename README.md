### 企业级系统开发 · AI 工具链

做指标体系与运营监控类系统，也折腾让 AI 真正能干活的工具链。

---

#### 技术栈

| | |
| :--- | :--- |
| **后端** | Java · Spring Boot 3 · JPA · Flyway · MySQL |
| **前端** | Vue 3 · Element Plus · Vite |
| **脚本** | Python · Shell · Docker |
| **方向** | MCP（Model Context Protocol）· 数据采集 · 告警与工单 |

---

#### 项目

**[mcp-servers](https://github.com/daijiaobu0306/mcp-servers)**　`Python`

两个 MCP 服务端，让 AI Agent 能操作 Linux 主机和 MySQL 数据库，同时把破坏性能力在代码层封死。

- `linux-mcp` — 沙箱内的文件操作与脚本执行：越界拦截、软删除、全量审计日志
- `mysql-mcp` — SQL AST 校验 + 关键字黑名单：`DROP` / `DELETE` / `TRUNCATE` 永久禁止，行数、超时、响应体积三重上限

---

#### 关注的方向

**工程规范**
数据库迁移有版本、可追溯；配置与代码分离；密钥永不入库。

**安全边界**
给自动化工具权限时，先想清楚它最坏能做什么，然后用代码把那条路堵死。

**可维护性**
文档要能当交接物用 —— 换个人、换个上下文，读完就能接着干。
