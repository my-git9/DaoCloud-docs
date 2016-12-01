---
title: 使用公有云的镜像市场添加主机
taxonomy:
    category:
        - docs
process:
    twig: true
---

为了方便用户部署，我们在国内的多家云主机厂商的应用市场中发布预置 DaoCloud 主机管理模块的虚拟机镜像。

要使用应用市场中的镜像模板，请参考下面的流程。

##### 腾讯云

要在腾讯云使用应用市场模板请参考下面的步骤：

1. 选择目标集群，点击「添加主机」
2. 点击「去买一台主机」，在列出的公有云清单中，选择您希望使用的，然后点击链接
3. 访问[腾讯云-服务市场](http://market.qcloud.com/detail.php?productId=143)并点击「立即使用」。在创建主机的界面也要记得选择系统类型为DaoCloud 混合容器（在服务市场中的 Docker 容器目录下）
4. 登录控制台找到新创建的云主机并点击「登录」。也可以通过 SSH 登录。
5. 获取绑定码后，在界面输入，并点击「完成」

![](qcloud-market.png)
![](qcloud2.png)
![](qcloud1.png)


就这么简单，这时您已经成功创建了一台腾讯云主机并和 DaoCloud 账户成功绑定了。您可以在集群中找到这台主机。阿里云和 UCloud 的操作，与上述腾讯云的方式类似，并且 DaoCloud 操作界面提供的非常清晰详尽的引导页面，这里就不再赘述。

>>>>> 完成公有云主机的添加后，您可以向公有云主机部署您的应用，或者从 DaoCloud 镜像仓库选择镜像部署，具体的操作步骤，请您参考[使用 DaoCloud 部署和管理应用](../../app-deploy-mgmt)这部分的文档内容。