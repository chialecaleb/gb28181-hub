# GB28181 Hub · 国标视频接入与管理平台

工程 / 目录 / 仓库名称：`gb28181-hub`。

GB28181 Hub 面向 GB/T 28181-2022 与 GB 35114-2017 的完整适用功能，提供独立视频接入与管理。接入采用 Java、Netty 和自研 JAIN SIP API 实现，管理采用 Spring Cloud Alibaba，前端采用 Vue 3 + TypeScript。

产品需求将 A / B / C 安全接入及级联、证书 / 密钥 / 安全媒体纳入必交付，并明确六协议输出、分屏轮巡、平台录像、用户资源权限、CAS / OAuth、开放 HTTP API、HTTPS 及 SQLite3 / MySQL / PostgreSQL 的设计和验收边界。代码和文档随 main 持续更新，不锁定与其他产品的组合版本。

- [需求文档](docs/requirements.md)：产品边界、协议能力、接入独立性、性能目标和验收条件。
- [设计文档](docs/design.md)：模块、SIP 内核、MQ 契约、集群路由、媒体、数据和部署设计。
- [标准资料与核对说明](docs/standards/README.md)：共享原始资料、页码、校验值和本产品规则职责。

本仓库自行维护实现、文档、协议规则、测试向量、依赖、配置和发布流程。开发及验收不以任何指定配套软件存在为前提。当前交付为文档基线，尚未完成软件实现或容量验证。

## 开发与文档入口

- [文档导航](docs/README.md)、[开发指令](AGENTS.md)与[开发指南](CONTRIBUTING.md)。
- [当前状态](docs/delivery/status.md)、[技术栈](docs/tech-stack.md)与[评审](REVIEW.md)。
- [用户事项入口](USER-ACTIONS.md)：导航到 workspace 的唯一清单。

当前可运行的统一检查：`python scripts/verify.py`（Python 3.10+、Git，仅 Python 标准库）。尚无应用启动命令。原始标准可单独获取，产品开发、构建和运行不依赖另一个产品仓库。
