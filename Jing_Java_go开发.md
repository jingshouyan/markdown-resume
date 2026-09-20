靖守彦 · Java/Go 架构师
========================

18 年经验 · 18552805073 · jingshouyan@gmail.com · 江苏徐州
1985.08 · 河海大学 本科 自动化（2003 届）
github.com/jingshouyan

----

专业摘要
--------

18 年一线研发经验，专注 Java 微服务架构与基础组件方向，兼具 Go 服务与工具链工程实践。主导自研企业级 RPC 框架（Dubbo + Thrift 扩展）、公司微服务框架与 Zookeeper 配置中心，支撑千万级消息量的私有化部署 IM 系统（10+ 微服务），长期负责核心服务的架构设计、编码实现、性能调优与线上问题排查。代表成果：消息服务重构 QPS 从 100+ 提升至 1000+；慢查询治理 p95 从 4000ms 降至 200ms；累计修复 CVE 安全漏洞 200+。近年持续实践 AI 编程，通过 Reasonix Code（DeepSeek）对话式开发完成完整小程序项目并开源。

----

核心技术栈
----------

编程语言
  Java / Kotlin（精通）：JVM 内存模型、GC 调优、多线程并发、NIO/Netty
  Go（熟练）：Goroutine/Channel、Gin、gorm、zorm、viper

框架与中间件
  RPC：Dubbo、Thrift、自研 J-RPC 框架
  微服务：SpringCloud、自研微服务框架
  ORM：MyBatis-Plus、JPA、Spring JDBC Template
  网络：Netty、NIO

存储与搜索
  MySQL：SQL 优化、B+ Tree 索引、慢查询治理（p95 4000ms → 200ms）
  国产数据库：达梦、金仓、神通
  Redis：缓存设计、分布式锁、缓存+数据同步（QPS 100+ → 1000+）
  ElasticSearch：分词、搜索
  Kafka：异步消息、削峰填谷

DevOps & 容器化
  Docker / K8s（裸机 → K8s 迁移）、GitLab CI、SonarQube、Harbor、Arthas

治理与安全
  自研 Zookeeper 服务注册发现与配置中心、CVE 漏洞修复 200+
  Helm、日志分析、监控系统

AI 编程
  Reasonix Code（DeepSeek）对话式编程完成完整项目交付
  驾考小程序 driver-exam-wx 从零到上线全流程

----

项目经验
========

一、信源密信 —— 企业级私有化部署 IM（Java 微服务）
北信源软件股份有限公司 · 2015.12 — 2026.06 · 基础服务组组长 / 架构师 · 管理团队 10+ 人

项目背景
  面向企业的私有化部署 IM 系统，分布式微服务架构，支持高并发与大规模用户访问。
  提供即时通讯、消息群发、消息存储、消息检索，以及开放平台 API（OA / CRM 等第三方集成）。

技术栈
  Java / Spring Boot · 自研微服务框架 · 自研 RPC（Dubbo + Thrift 扩展）· Zookeeper · MySQL · Redis · K8s

核心工作

  【1】消息服务重构 —— QPS 100+ → 1000+
      引入缓存 + 数据同步技术重构消息服务，QPS 从 100+ 提升至 1000+（10 倍提升）。

  【2】微服务治理 —— 服务数量 -30%
      按业务边界拆分为用户、登录、在线、群组、好友、ID、消息、云推送等 10+ 独立微服务；
      主导服务内聚合并与重构，服务数量减少 30%，调用链显著缩短，系统稳定性提升。

  【3】性能优化 —— p95 4000ms → 200ms
      定位核心服务慢查询与复杂查询问题并完成治理，p95 延时从 4000ms 降至 200ms。

  【4】自研 RPC 框架（Dubbo + Thrift 扩展）
      统一公司服务间调用协议；Spring Boot Starter 一键接入；内置 Zipkin 调用链追踪、
      请求/响应数据脱敏；负责架构设计、核心功能开发与性能优化。

  【5】自研微服务框架与配置中心
      公司微服务框架的设计开发与维护；自研基于 Zookeeper 的服务注册发现与配置中心，
      支持动态配置下发，设计三方组件动态接入方案。

  【6】部署升级与 CI/CD
      服务部署从裸机迁移至 K8s；搭建 GitLab CI 全链路流水线：
      K8s Runner + Minio 缓存 + SonarQube 代码质量检查 + Harbor 镜像仓库。

  【7】安全治理
      Java 第三方依赖管理，累计修复 CVE 安全漏洞 200+，完成依赖版本与构建工具升级。

  【8】开放平台与 AI 集成
      设计开放平台 API，支持 OA / CRM 等第三方系统对接；接入 AI 能力平台（Cli、OpenClaw）。

二、Go 服务与工具链
北信源软件股份有限公司 · 2021 — 2025

  【1】日志分析工具（Go）
      处理海量服务日志，支持实时检索与告警。

  【2】cve-analyzer（Go CLI）· github.com/jingshouyan/cve-analyzer
      解析 OWASP dependency-check 输出的 CSV 漏洞报告，生成 CSV + Markdown 结构化摘要；
      支持建议字段自定义维护、多次生成保留历史记录。

  【3】nvd-data-mirror（Go 服务）· github.com/jingshouyan/nvd-data-mirror
      为 dependency-check-maven 提供 CVE 与 RetireJS 数据镜像，减少对 NVD 官方源的依赖，
      提升数据获取的稳定性与速度。

三、钱生钱小额贷款系统（Java）
钱袋宝软件股份有限公司 · 2014.05 — 2015.12

项目背景
  小额贷款全流程系统（申请 / 审批 / 放款 / 还款）+ 对账系统 + 管理平台。

核心工作
  · 核心功能开发、性能优化与故障排查
  · 对接多家银行系统接口，保障数据准确传输与处理
  · 设计开发对账系统，保障数据准确性与一致性
  · 设计开发管理平台，支撑运营与风控团队

----

工作经历
--------

北信源软件股份有限公司 · 基础服务组组长 / 架构师 · 2015.12 — 2026.06
  负责公司基础架构层的设计与维护：IM 系统、微服务框架、RPC 框架、配置中心、CI/CD 流水线。管理团队 10+ 人。

钱袋宝软件股份有限公司 · Java 研发工程师 · 2014.05 — 2015.12
  小额贷款系统、银行接口对接、对账系统、管理平台。

淮海中联水泥有限公司 · 信息中心 IT 技术工程师 · 2008.08 — 2014.05
  ERP 系统维护、内部需求分析与供应商协调、IT 基础设施维护（网络、服务器、数据库）。

----

个人开源项目
------------

J-RPC — 基于 Thrift 的 JSON 格式 RPC 框架
github.com/jingshouyan/j-rpc · 2018.08 — 2021.06
轻量级 RPC 框架，Zookeeper 注册发现。Spring Boot Starter 零配置接入，支持 Zipkin 追踪、数据脱敏、自动生成 API 文档、JMeter 压测。

J-JDBC — Spring JDBC Template CRUD 增强
github.com/jingshouyan/j-jdbc · 2018.04 — 2021.04
基于注解的 CRUD 增强，支持动态 SQL、多数据库方言（MySQL、达梦、金仓等）、字段加密存储。

driver-exam-wx — 驾考科目一/四 微信小程序
github.com/jingshouyan/driver-exam-wx · 2026.06
刷题学习小程序，含顺序练习、模拟考试、错题本。全程 Reasonix Code（DeepSeek）AI 编程完成。

（cve-analyzer、nvd-data-mirror 见上方「项目经验 · Go 服务与工具链」）

----

