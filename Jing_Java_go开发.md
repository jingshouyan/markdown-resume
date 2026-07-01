靖守彦 · Java/Go 架构师
========================

18 年经验 · 18552805073 · jingshouyan@gmail.com · 江苏徐州
1985.08 · 河海大学 本科 自动化（2003 届）
github.com/jingshouyan

----

专业摘要
--------

18 年后端开发经验，专注于 Java/Go 分布式系统基础架构方向。主导自研了基于 Dubbo + Thrift 扩展的企业级 RPC 框架，支撑千万级消息量的私有化部署 IM 系统。具备微服务治理、容器化迁移（裸机 → K8s）、DevOps 全链路搭建、国产数据库适配等落地经验。擅长基础组件设计与性能调优：消息服务重构 QPS 从 100+ 提升至 1000+，慢查询治理 p95 延时从 4000ms 降至 200ms。累计修复 CVE 安全漏洞 200+。积极探索 AI 编程实践，通过 Reasonix Code（DeepSeek）对话式开发完成完整小程序项目。

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

工作经历
--------

北信源软件股份有限公司 · 基础服务组组长 / 架构师
2015.12 — 2026.06 · 管理团队 10+ 人

负责公司基础架构层的设计与维护，涵盖 IM 系统、微服务框架、RPC 框架、配置中心、CI/CD 流水线等。

核心项目：信源密信（企业级私有化部署 IM）

架构设计与治理
  · 将 IM 系统拆分为用户/登录/在线/群组/好友/ID/消息/云推送等 10+ 微服务
  · 服务内聚合并与重构，服务数量减少 30%，调用链显著缩短
  · 消息服务重构（缓存+数据同步），QPS 从 100+ 提升至 1000+
  · 主导部署模式从裸机迁移至 K8s

自研基础设施
  · RPC 框架：基于 Dubbo + Thrift 扩展，统一服务间调用协议，Spring Boot Starter 集成、Zipkin 追踪、数据脱敏
  · 配置中心：基于 Zookeeper 的服务注册发现与配置中心，支持动态配置下发
  · JDBC 增强工具：基于 Spring JDBC Template 自研 CRUD 增强框架（开源 J-JDBC）

DevOps & 工程效率
  · GitLab CI 全链路：K8s Runner + Minio + SonarQube + Harbor
  · Java 依赖管理，CVE 漏洞修复 200+，构建工具升级

Go 工具链开发
  · 日志分析工具（Go）：海量日志实时检索与告警
  · cve-analyzer（Go CLI）：自动解析 OWASP 依赖检查报告
  · nvd-data-mirror（Go 服务）：CVE 数据国内镜像

开放平台 & AI 集成
  · 设计开放平台 API，对接 OA/CRM 等第三方系统
  · 对接 AI 平台（Cli、OpenClaw）

----

钱袋宝软件股份有限公司 · Java 研发工程师
2014.05 — 2015.12

项目：钱生钱小额贷款系统
  · 核心功能开发、性能优化
  · 对接多家银行接口
  · 设计开发对账系统
  · 设计开发管理平台

----

淮海中联水泥有限公司 · 信息中心 IT 技术工程师
2008.08 — 2014.05

  · ERP 系统维护与故障排查
  · 内部需求分析与供应商协调
  · IT 基础设施维护（网络、服务器、数据库）

----

个人开源项目
------------

J-RPC — 基于 Thrift 的 JSON 格式 RPC 框架
github.com/jingshouyan/j-rpc · 2018.08 — 2021.06
轻量级 RPC 框架，Zookeeper 注册发现。Spring Boot Starter 零配置接入，支持 Zipkin 追踪、数据脱敏、自动生成 API 文档、JMeter 压测。

J-JDBC — Spring JDBC Template CRUD 增强
github.com/jingshouyan/j-jdbc · 2018.04 — 2021.04
基于注解的 CRUD 增强，支持动态 SQL、多数据库方言（MySQL、达梦、金仓等）、字段加密存储。

cve-analyzer — CVE 漏洞报告分析工具（Go）
github.com/jingshouyan/cve-analyzer · 2021.05 — 2025.04
解析 OWASP dependency-check 输出的 CSV 漏洞报告，生成结构化摘要。

nvd-data-mirror — NVD 数据镜像服务（Go）
github.com/jingshouyan/nvd-data-mirror · 2021.04 — 2024.03
为 dependency-check-maven 提供 CVE 和 RetireJS 国内镜像。

driver-exam-wx — 驾考科目一/四 微信小程序
github.com/jingshouyan/driver-exam-wx · 2026.06
刷题学习小程序，含顺序练习、模拟考试、错题本。全程 Reasonix Code（DeepSeek）AI 编程完成。


