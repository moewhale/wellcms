## 中文 / Chinese

### 简介
WellCMS 3.0 是一款基于现代 PHP 架构的内容管理系统，支持插件扩展、主题定制、数据库分片及任务调度。

### 核心特性
- **现代 PHP 架构**：基于 PSR-7 HTTP 标准、依赖注入容器与服务提供者模式
- **插件系统**：支持插件的安装、卸载、启用与市场接入
- **主题机制**：支持父子主题继承与自定义模板
- **数据库能力**：连接池、读写分离、分库分表与分区维护
- **任务调度**：内置调度器，支持定时任务与队列执行
- **多语言支持**：内置 14 种语言包
- **缓存体系**：支持 Redis、Memcached、APCu、Yac 等多种缓存驱动
- **安全管理**：CSRF、XSS、权限、Token、IP 黑名单等多重安全机制
- **Swoole 支持**：提供 Swoole Server 与协程环境下的运行能力

### 安装方式
1. 将代码部署到 Web 根目录
2. 将 `src/Config/*.default.php` 复制为 `config/*.php` 并按需配置
3. 访问 `/install/` 完成数据库安装

### 系统要求
- PHP >= 8.0
- MySQL / MariaDB / PostgreSQL / SQLite
- Redis（可选，用于缓存与任务队列）

### 注意事项
- 此为首个版本，建议用于测试与评估环境
- 生产部署前请仔细阅读 `bin/SWOOLE_DEPLOY_GUIDE.md` 与 `bin/SCHEDULER_DEPLOY_GUIDE.md`

---

## English

### Introduction
WellCMS 3.0 is a content management system built on modern PHP architecture, supporting plugin extensions, theme customization, database sharding, and task scheduling.

### Key Features
- **Modern PHP Architecture**: PSR-7 HTTP standard, dependency injection container, and service provider pattern
- **Plugin System**: Install, uninstall, enable plugins, and connect to the plugin market
- **Theme Mechanism**: Parent-child theme inheritance and custom templates
- **Database Capabilities**: Connection pooling, read/write splitting, sharding, and partition maintenance
- **Task Scheduling**: Built-in scheduler supporting cron jobs and queue execution
- **Multi-language Support**: 14 built-in language packs
- **Caching System**: Redis, Memcached, APCu, Yac, and more cache drivers
- **Security Management**: CSRF, XSS, permissions, tokens, IP blacklist, and more
- **Swoole Support**: Swoole Server and coroutine runtime support

### Installation
1. Deploy the code to your web root directory
2. Copy `src/Config/*.default.php` to `config/*.php` and configure as needed
3. Visit `/install/` to complete database installation

### Requirements
- PHP >= 8.0
- MySQL / MariaDB / PostgreSQL / SQLite
- Redis (optional, for caching and task queues)

### Notes
- This is the first release, recommended for testing and evaluation environments
- For production deployment, please read `bin/SWOOLE_DEPLOY_GUIDE.md` and `bin/SCHEDULER_DEPLOY_GUIDE.md` first
