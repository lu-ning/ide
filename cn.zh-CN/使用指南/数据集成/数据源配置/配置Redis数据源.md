# 配置Redis数据源 {#concept_t3r_4tb_p2b .concept}

Redis是文档型的NoSQL数据库，提供持久化的内存数据库服务，基于高可靠双机热备架构及可无缝扩展的集群架构，满足高读写性能场景及容量需弹性变配的业务需求。Redis数据源提供了读取和写入Redis双向通道的能力，可以通过脚本模式配置同步任务。

## 操作步骤 {#section_jy4_q4v_42b .section}

1.  以项目管理员身份进入[DataWorks管理控制台](https://workbench.data.aliyun.com/console)，单击对应项目操作栏中的**进入数据集成**。
2.  单击**数据源** \> **新增数据源**，弹出支持的数据源。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/16212/15421915407592_zh-CN.png)

3.  在新建数据源弹出框中，选择数据源类型为**Redis**。
4.  配置Redis数据源的各个信息项。

    Redis的数据源类型分为**阿里云数据库**和**有公网IP的自建数据库**。

    -   阿里云数据库：一般使用的网络是经典网络类型，同地区的经典网络能连通，跨地区的经典网络连接不保证能通。
    -   有公网IP的自建数据库：一般使用的网络是公网，然而公网可能产生一定的费用。
    以新增**Redis** \> **阿里云数据库**类型的数据源为例。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/16212/15421915407593_zh-CN.png)

    配置项说明如下：

    -   数据源类型：当前选择的数据源类型为Redis\>阿里云数据库。

        **说明：** 如果您尚未授权数据集成系统默认角色，需要主账号前往RAM对角色进行授权，然后刷新此页面。

    -   数据源名称： 由英文字母、数字、下划线组成且需以字符或下划线开头，长度不超过60个字符。
    -   数据源描述： 对数据源进行简单描述，不得超过80个字符。
    -   地区：是指在购买Redis时所选的区域。
    -   Redis实例ID：您可进入Redis管控台查看Redis实例ID。
    -   Redis访问密码：Redis Server的访问密码，如果没有则不填。
    以新增**Redis** \> **有公网IP的自建数据库**类型的数据源为例。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/16212/15421915407594_zh-CN.png)

    配置项说明如下：

    -   数据源类型：当前选择的数据源类型为Redis\>有公网IP的自建数据库。
    -   数据源名称： 由英文字母、数字、下划线组成且需以字符或下划线开头，长度不超过60个字符。
    -   数据源描述： 对数据源进行简单描述，不得超过80个字符。
    -   服务器地址：格式为host:port 。
    -   添加访问地址：添加访问地址，格式为host:port 。
    -   Redis访问密码：Redis的服务访问密码。
5.  单击**测试连通性**。
6.  测试连通性通过后，单击**确定**。

## 后续步骤 { .section}

现在，您已经学习了如何配置Redis数据源，您可以继续学习下一个教程。在该教程中您将学习如何通过配置Redis Writer插件。详情请参见 [配置Redis Writer](intl.zh-CN/使用指南/数据集成/作业配置/配置Writer插件/配置Redis Writer.md#)。

