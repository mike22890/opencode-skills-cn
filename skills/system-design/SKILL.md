---
name: system-design
description: 系统设计/架构/微服务/数据库/缓存/分布式/CAP/高并发/DevOps 时触发。
version: 1.0.0
metadata:
  author: opencode-skills-cn
  tags: system-design architecture microservices distributed devops sre scalability
---

# System Design（系统设计）

## 何时触发

关键词命中即触发：系统设计、架构、微服务、数据库、缓存、队列、负载均衡、分布式、高并发、高可用、DevOps、SRE、可观测性、监控、部署、K8s、容器、扩展、一致性、CAP、BASE。

## 速记 6 条

1. **CAP**：一致性 / 可用性 / 分区容错三选二
2. **水平扩展**：加机器优于加配置
3. **异步优于同步**：队列解耦
4. **幂等性**：可重试 = 安全
5. **可观测性**：日志 + 指标 + 链路
6. **降级熔断**：失败要优雅

## 自检清单

- [ ] 是否考虑了分区容错？
- [ ] 是否异步解耦关键路径？
- [ ] 是否有缓存 + 防穿透 / 雪崩 / 击穿？
- [ ] 是否幂等可重试？
- [ ] 是否有可观测性（日志 / 指标 / 链路）？
- [ ] 是否有降级 / 熔断方案？
- [ ] 是否考虑 10x / 100x 流量？

## 加载 reference

| 用户说 | 加载 |
|---|---|
| CAP / BASE / 一致性 / 分区 / 复制 | `reference/principles.md` |
| 微服务 / 事件驱动 / CQRS / Saga / 限流 | `reference/patterns.md` |
| 缓存 / 队列 / 数据库 / CDN / 监控 | `reference/scale.md` |
| 学谁 / 大师 / 锚点 | `reference/masters.md` |
