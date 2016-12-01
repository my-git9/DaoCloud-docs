---
title: 添加胶囊主机
taxonomy:
    category:
        - docs
process:
    twig: true
---

如果您还没有一台装有 Linux 的主机，我们邀请您体验「免费胶囊主机」。

要启动一台胶囊主机请参考下面的步骤：

1. 在控制台点击「我的集群」
2. 选择一个目标集群，或者创建一个新的集群
3. 点击添加主机
4. 在接入自有主机界面，将鼠标移到「先试试胶囊主机」，点击「试用」

![](jiaonang.png?resize=800)

> 「胶囊主机」自带 Docker 运行环境，并自动接入 DaoCloud 容器管理平台。每个「胶囊主机」可以免费体验 120 分钟，到期后会自动消失。「胶囊主机」到期后可以再次体验。

创建胶囊主机后，您可以在弹出的提醒窗口中，点击「查看新主机」，在此界面，您可以查看和完成如下操作：

![](jiaonang-mgmt.png?resize=800)

1. 查看主机的 IP 地址
2. 查看主机的连接状态，在胶囊主机被创建后，主机会花约 10 秒时间，与 DaoCloud 平台建立连接，连接完成后，会显示主机上的 Docker 版本，和绿色的「运行正常」字样
3. 我们允许用户通过 SSH 方式登录主机，在主机管理界面，可以看到 SSH 连接的方式，包括 IP、用户名和密码
4. 页面右上角显示了胶囊主机的可用时间
5. 如果您在胶囊主机上部署应用，还可以在下方的界面显示容器清单

胶囊主机安装了 Docker ，是您上手操作练习的最佳平台，我们建议您浏览 Docker 公司网站，在胶囊主机上熟悉各类基本 Docker 命令。

>>>>> 胶囊主机也可以用来部署应用，但请您一定注意备份数据，胶囊主机会在 120 分钟生命周期达到后自动销毁。您可以添加任意数量的胶囊主机。

返回集群管理界面，您会看到集群中已经增加了一台主机，我们在集群的管理界面，会显示当前主机的 CPU、内存、磁盘和 Docker 版本、运行状态等关键信息。

![](cluster-status.png?resize=800)

>>>>> 完成胶囊主机的添加后，您可以向胶囊主机部署您的应用，或者从 DaoCloud 镜像仓库选择镜像部署，具体的操作步骤，请您参考[使用 DaoCloud 部署和管理应用](../../app-deploy-mgmt)这部分的文档内容。