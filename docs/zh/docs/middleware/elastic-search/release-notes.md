# Elasticsearch 索引服务 Release Notes

本页列出 Elasticsearch 索引服务的 Release Notes，便于您了解各版本的演进路径和特性变化。

## v0.3.4

发布日期：2022-10-28

- **新增** 同步 pod 状态到实例详情页
- **优化** workspace 界面逻辑调整
- **优化** 不符合设计规范的样式调整
- **优化** password 获取逻辑调整
- **优化** cpu&内存请求量应该小于限制量逻辑调整
- **优化** 实例版本不允许修改，下拉框应该为文本
- **修复** 更新实例服务设置，确认无反应，无法提交
- **新增** 获取用户列表接口
- **新增** 支持 arm 架构

## v0.3.2

发布日期：2022-9-25

### API

- **新增** 列表页增加分页功能
- **新增** 增加修改配置的功能
- **新增** 增加返回可修改配置项的功能
- **新增** 更改创建实例的限制为集群级别，原来为 namespace 级别
- **新增** 增加监控地址的拼接功能
- **新增** 增加可以修改版本号的功能
- **新增** 修改底层 update 逻辑为 patch 逻辑
- **新增** 将时间戳 api 字段统一调整为 int64
- **新增** 单测覆盖率提升到 43%
- **新增** 对接全局管理增加 workspace 接口
- **新增** 对接 insight 通过 crd 注入 dashboard
- **新增** 更新 release note 脚本，执行 release-process 规范

### 安装

- **新增** 支持 helm 部署 eck-operator
- **新增** 支持 helm 部署 mcamel-elasticsearch 服务

### 文档

- **新增** 第一次文档网站发布
- **新增** 功能说明
- **新增** 产品优势
- **新增** 什么是 Elasticsearch
- **新增** 基本概念
- **新增** 集群容量规划