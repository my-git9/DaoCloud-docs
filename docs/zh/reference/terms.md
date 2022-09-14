# 术语表

本页介绍 DEC 5.0 各个模块中的常见术语。

- 服务发现

    用于 Kubernetes 环境的服务发现配置，用于批量且自动地接入 Kubernetes 上的监控点。

- 服务网格 (Service Mesh)
    
    服务网格是在网络层 TCP/IP 上建立的一个中间层，接管服务之间的通信流量，将微服务治理能力下沉，从而实现对上层应用透明、不限制语言、无侵入的享受微服务能力。使用服务网格时，通过还会在应用服务旁边注入一个 SideCar 代理，实现对服务网络流量的拦截。

- 告警规则

    基于资源状态创建告警对象，自定义触发规则的条件以及通过何种方式发送通知的规则。

- Grafana

    Grafana 是一个开源的可视化平台，提供了多样的监控数据可视化面板。

- 汇总（Summary）

    类似于直方图，汇总也对观察结果进行采样。除了可以统计采样值总和和总数，它还能够按分位数统计。有以下几种方式来产生汇总（假设度量指标为 `<basename>`）：

    - 按分位数，也就是采样值小于该分位数的个数占总数的比例小于 φ，相当于 `<basename>{quantile="<φ>"}`
    - 采样值总和，相当于 `<basename>_sum`
    - 采样值总数，相当于 `<basename>_count`

- 计量器（Gauge）

    计量器是一个**既可增又可减**的度量指标值。计量器主要用于测量类似于温度、内存使用量这样的瞬时数据。

- 计数器（Counter）

    计数器是一种累计型的度量指标，它是一个**只能递增**的数值。计数器主要用于统计类似于服务请求数、任务完成数和错误出现次数这样的数据。

- 链路

    记录单次请求范围内的处理信息，其中包括服务调用和处理时长等数据。一个 Trace 有一个唯一的 Trace ID ，并由多个 Span 组成。

- 目标

    Prometheus 抓取的采集目标。采集目标暴露自身状态，或者代理暴露监控对象的运行、业务指标。

- Prometheus

    Prometheus是一套开源的监控、报警、时间序列数据库的组合。

- PromQL

    Prometheus 内置的数据查询语言，其提供对时间序列数据丰富的查询，聚合以及逻辑运算能力的支持。

- 日志

    系统运行过程中变化的一种抽象数据，其内容为指定对象的操作和其操作结果按时间的有序集合。

- 审计日志

    审计日志提供了对系统中对象所做更改的历史记录。

- 通知

    当资源存在异常而产生告警时，可将告警信息通过邮件、钉钉、企业微信、webhook等方式发送给指定的用户。

- 直方图（Histogram）

    直方图对观察结果（通常是请求持续时间或者响应大小这样的数据）进行采样，并在可配置的桶中对其进行统计。有以下几种方式来产生直方图（假设度量指标为 `<basename>`）：

    - 按桶计数，相当于 `<basename>_bucket{le="<upper inclusive bound>"}`
    - 采样值总和，相当于`<basename>_sum`
    - 采样值总数，相当于 `<basename>_count` ，也等同于把所有采样值放到一个桶里来计数 `<basename>_bucket{le="+Inf"}`

    Histogram 可以理解为柱状图，典型的应用如：请求持续时间，响应大小。可以对观察结果采样，分组及统计。

- 指标

    对资源性能的数据描述或状态描述，指标由命名空间、维度、指标名称和单位组成。采集目标暴露的、可以完整反映监控对象运行或者业务状态的一系列标签化数据。