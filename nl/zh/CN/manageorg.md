---

copyright:

  years: 2015, 2018
lastupdated: "2018-01-23"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# 使用组织
作为帐户所有者或组织管理员，您可以执行组织管理任务，包括重命名组织、删除组织或空间、更新组织或空间角色以及管理配额和域。
{:shortdesc}

要在 {{site.data.keyword.Bluemix}} 控制台中管理组织，请单击**管理 > 帐户 > Cloud Foundry 组织**。一次只能查看一个组织的资源。如果您是多个组织的成员，那么可以通过控制台菜单栏中的用户帐户首选项链接来切换组织。

## 重命名组织
{: #orgrename}

要重命名组织，请完成以下步骤：
1. 单击**管理** > **帐户** > **Cloud Foundry 组织**。
2. 确定要重命名的组织，然后单击**查看详细信息**。
3. 单击**编辑 Cloud Foundry 组织**。
4. 单击组织名称旁边的**编辑**。
5. 输入新的组织名称，然后单击**保存**。

## 删除组织和空间
{: #deleteorgs}

### 删除组织

删除组织时，会删除该组织内的所有空间、应用程序和服务。请务必注意，删除操作不可撤销。 

### 删除空间

要删除空间，请完成以下步骤：

1. 单击**管理** > **帐户** > **Cloud Foundry 组织**。
2. 选择要编辑的组织，然后单击**查看详细信息**。
3. 确定要删除的空间，然后单击**编辑空间**。
4. 单击**删除 Cloud Foundry 空间**。

## 编辑用户角色
{: #listmembers}

### 编辑特定组织的用户角色 

要编辑特定组织的用户角色，请完成以下步骤：

1. 单击**管理** > **帐户** > **Cloud Foundry 组织**。
2. 确定要编辑的组织，然后单击**查看详细信息**，再单击**编辑组织**。
4. 在**用户**选项卡中可以看到组织成员及其角色。

### 编辑特定空间的用户角色

要编辑特定空间的用户角色，请完成以下步骤：

1. 单击**管理** > **帐户** > **Cloud Foundry 组织**。
2. 选择要查看其成员的组织，然后单击**查看详细信息**。
3. 确定要编辑的空间，然后单击**编辑空间**。
4. 在**用户**选项卡中可以查看空间成员及其角色。

## 管理配额
{: #managequota}

作为 {{site.data.keyword.Bluemix_notm}} 帐户所有者或组织管理员，您可以查看组织的已使用和已分配配额。配额表示创建组织时为其分配的资源限制。组织可用的资源根据您是具有免费帐户还是计费帐户而有所不同。组织内空间中的任何应用程序或服务都会使用一定的已分配配额。

要查看组织的已使用和已分配配额，请完成以下步骤：

1. 单击**管理** &gt; **帐户** &gt; **Cloud Foundry 组织**。
2. 确定要查看其配额的组织，然后单击**查看详细信息**。
3. 单击**编辑组织**。
4. 如果您已在多个区域中定义空间，请选择要查看的特定区域。
5. 单击**配额**。 
6. 缺省情况下会打开 **Cloud Foundry** 配额页面。您可以查看以下资源的配额详细信息：

 * 内存
 * 服务
 * 套餐
 * 价格
7. 单击**容器**以查看已用和可用的容器配额分配。容器分配根据价格套餐而有所不用。您可以查看以下资源的配额详细信息：

 * 内存
 * 公共 IP
 * 文件共享
8. 单击**虚拟服务器**以查看虚拟机。

在 {{site.data.keyword.Bluemix_notm}} 悉尼区域中无法使用容器。
{: tip}

有关容器的更多信息，请参阅“容器”文档中的[配额](/docs/containers/container_planning.html#container_planning_quota)。
要更改为组织所分配的配额，必须开具支持凭单。有关开具支持凭单的更多信息，请参阅[获取客户支持](/docs/get-support/howtogetsupport.html#getting-customer-support)。 

## 管理域
{: #managedomains}

作为 {{site.data.keyword.Bluemix_notm}} 帐户所有者或组织管理员，您可以针对组织及其空间内构建的应用程序，查看其系统域并为其添加定制域。作为空间管理员，空间的**域**选项卡是分配给该空间的域的只读列表。

1. 单击**管理** &gt; **帐户** &gt; **Cloud Foundry 组织**。
2. 确定要查看或编辑其域的组织。
3. 对该组织选择**查看详细信息**。
4. 单击**编辑组织**。
5. 单击**域**。

如果您添加定制域，那么必须配置 DNS 服务器以将您的定制域解析为指向 {{site.data.keyword.Bluemix_notm}} 系统域。这样，当 {{site.data.keyword.Bluemix_notm}} 接收到定制域的请求时，它可以将其正确路由到您的应用程序。系统域始终可供空间使用，另外还可为空间分配定制域。空间中创建的应用程序可使用为该空间列出的任何域。有关创建和使用定制域的更多信息，请参阅[使用定制域](/docs/apps/updapps.html#domain)。