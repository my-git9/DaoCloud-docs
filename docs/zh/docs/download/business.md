# DCE 5.0 商业版

本页可下载 DCE 5.0 商业版的离线安装包和校验文件。

## 下载

| 版本名称 | 文件大小 | 下载                                                                                                        |
| -------- | -------- | ----------------------------------------------------------------------------------------------------------- |
| 离线包   | 21 GB    | [点击下载](https://qiniu-download-public.daocloud.io/DaoCloud_Enterprise/dce5/offline-v0.3.28.tar)          |
| 校验文件 | 0.1 KB   | [点击下载](https://qiniu-download-public.daocloud.io/DaoCloud_Enterprise/dce5/offline-v0.3.28-checksum.txt) |

## 安装和授权

下载完整离线包之后，请参阅[商业版安装流程](../install/Air-Gap-install-full/start-install.md)。

## 包含的模块

DCE 5.0 社区版默认包含以下模块：

| 模块       | 介绍                                                                     | 最新动态                                                   |
| ---------- | ------------------------------------------------------------------------ | ---------------------------------------------------------- |
| 全局管理   | 负责用户访问控制、权限、企业空间、审计日志、个性化外观设置等             | [发布说明](../release/rn5.0.md#_4)                         |
| 容器管理   | 管理集群、节点、工作负载、Helm 应用、CRD、命名空间等 K8s 核心功能        | [v0.12.0](../kpanda/03ProductBrief/release-notes.md#v0120) |
| 可观测性   | 提供丰富的仪表盘、场景监控、数据查询、告警等图文信息                     | [v0.11.1](../insight/03ProductBrief/releasenote.md#v0111)  |
| 应用工作台 | 基于容器的 DevOps 应用平台，支持 Jenkins, Tekton, GitOps 等流水线作业    | [发布说明](../amamba/01ProductBrief/releasenote.md)        |
| 多云编排   | 集中管理多云、混合云、跨云资源的应用编排，具备多云灾备、故障恢复等能力   | [v0.3.0](../kairship/01product/release-notes.md)           |
| 微服务引擎 | 提供注册发现、服务治理、配置管理、微服务网关等治理能力                   | [发布说明](../release/rn5.0.md)                            |
| 服务网格   | 基于 Istio 开源技术构建的面向云原生应用的下一代服务网格                  | [v0.10.0](../mspider/01Intro/release-notes.md)             |
| 中间件     | 包含 RabbitMQ、Kafka、Elasticsearch、MySQL、Redis、MinIO 等精选中间件    | [发布说明](../release/rn5.0.md)                            |
| 镜像仓库   | 用于存储 K8s、DevOps 和容器应用开发的镜像                                | [发布说明](../release/rn5.0.md)                            |
| 网络       | 针对不同的 Linux 内核，支持多种 CNI 组合方案                             | [发布说明](../release/rn5.0.md)                            |
| 存储       | 提供统一数据存储服务，支持文件、对象、块、本地存储，轻松接入存储厂商方案 | [发布说明](../release/rn5.0.md)                            |

## 更多

- [在线文档](https://docs.daocloud.io/dce/what-is-dce/)
- [报告 bug](https://github.com/DaoCloud/DaoCloud-docs/issues)