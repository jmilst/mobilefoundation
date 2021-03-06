---

copyright:
  years: 2018
lastupdated: "2018-11-22"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:tip: .tip}
{:note: .note}
{:pre: .pre}
{:codeblock: .codeblock}
{:screen: .screen}

# 在控制台上可视化洞察
{: #visualize_insights_on_console}

在 MobileFirst Analytics 控制台中，可以查看和配置分析报告，管理警报以及查看客户机日志。在 Mobile Foundation Operations Console 中，通过单击左侧导航中的 **Analytics 控制台**来启动 Analytics 控制台。

这将启动 Analytics 控制台，并且会显示缺省仪表板。如果客户机应用程序已将日志和分析数据发送到服务器，那么将创建并显示相关报告。在仪表板中，可以复查所收集的分析数据。这些分析数据可能与应用程序崩溃、应用程序会话和服务器处理时间相关。此外，可以创建定制图表并管理警报。

除了 Mobile Analytics 的概览视图外，分析功能还包括对客户机日志、捕获的客户机崩溃数据以及通过向 Mobile Analytics 提供数据的客户机 API 函数调用显式提供的任何额外数据执行原始搜索的功能。

## 监视应用程序数据
{: #monitoring_app_data}

Mobile Analytics 为移动应用程序提供监视和分析功能。您可以使用 Mobile Analytics 客户机 SDK 来记录应用程序日志和监视数据。开发者可以控制何时将这些数据发送到 Mobile Analytics 服务。将数据传递到 Mobile Analytics 后，可以使用 Mobile Analytics 控制台来获取有关移动应用程序、设备和应用程序日志的分析洞察。

可以推断出的一些洞察如下：

**预定义的度量值**

通过预定义的度量值，可以回答如下问题：
* 我有多少位新用户？
* 使用应用程序的活跃用户有多少？
* 用户使用应用程序的频率如何？
* 用户在一天中的什么时间使用应用程序？
* 用户偏好什么设备型号？
* 我应该何时弃用对旧操作系统的支持？
* 哪些应用程序遇到了性能问题？

**定制事件**

通过添加您自己的定制事件，可以回答如下问题：
* 哪些功能最常用，哪些最不常用？
* 用户在哪里进入我的应用程序，又在哪里离开？
* 用户查看最多的活动是哪些？
* 用户是否在应用程序中完成工作流程（例如，转换漏斗）？

## 可以可视化的报告：用户
{: #reports_visualized_users}

此报告展示的图表显示指定日期范围内已使用应用程序的活跃用户数。报告还显示指定日期范围内首次使用应用程序的非重复新用户数。可以按应用程序名称、操作系统或操作系统版本对这些图表进行过滤。

## 可以可视化的报告：会话
{: #reports_visualized_sessions}

此报告展示的图表显示指定日期范围内的应用程序会话数。在应用程序进入设备前台时会记录一次会话。可以按应用程序名称、操作系统或操作系统版本对这些图表进行过滤。

## 可以可视化的报告：网络请求
{: #reports_visualized_network_requests}

在 Mobile Analytics 控制台中对应用程序的网络请求数据进行可视化。

数据可用于以下度量：

**往返时间** - 定义应用程序发出网络请求所用的时间长度（以毫秒为单位度量）。**请求计数** - 显示应用程序发出网络请求的频率。数据还显示为平均值。可以按应用程序名称、操作系统或操作系统版本对这些图表进行过滤。

## 可以可视化的报告：崩溃
{: #reports_visualized_crashes}

可以在 Mobile Analytics 控制台中查看有关应用程序崩溃的信息，以便更好地对应用程序进行监视和故障诊断。

在“崩溃”页面上，**崩溃概述**表显示以下数据列：

**应用程序**：应用程序名称<br/>
**崩溃次数**：该应用程序的崩溃总次数<br/>
**总使用次数**：用户打开并关闭该应用程序的总次数<br/>
**崩溃率**：每次使用的崩溃百分比<br/>
您可以在崩溃表中快速查看有关应用程序崩溃的信息。“崩溃”条形图显示崩溃次数随时间变化的直方图。<br/>

可以使用两种方式来显示崩溃数据：

1.  显示崩溃率：随时间变化的崩溃率
2.  显示崩溃总次数：随时间变化的崩溃总次数

## 可以可视化的报告：故障诊断
{: #reports_visualized_troubleshooting}

Mobile Analytics 控制台中的**故障诊断**页面使用**崩溃摘要**表提供了应用程序崩溃的详细视图。

**崩溃摘要**表可排序，包含以下数据列：

* 崩溃次数
* 设备数
* 上次崩溃时间
* 应用程序
* 操作系统
* 消息

单击任意条目旁的 + 图标，以显示包含以下各列的**崩溃详细信息**表：

* 崩溃时间
* 应用程序版本
* 操作系统版本
* 设备型号
* 设备标识
* 下载：用于下载崩溃前的日志的链接

展开**崩溃详细信息**表中的任何条目，以获取包含堆栈跟踪在内的更多详细信息。

**崩溃摘要**表的数据是通过查询致命级别应用程序日志来填充的。如果应用程序未收集致命应用程序日志，那么不会有数据可用。
{: note}


## 可以可视化的报告：用户反馈
{: #reports_visualized_userfeedback}

“用户反馈”提供使用 Mobile Analytics 进行的应用程序内反馈分析。通过 Mobile Analytics 的此功能 - 
* **用户和测试者**可以在运行和使用应用程序时，记录并发送来自应用程序的反馈和错误报告。
* **应用程序所有者**通过这一富含上下文的用户反馈，可以更深入了解应用程序的用户体验。
* 但是，**开发者**可收到准确的应用程序上下文，以诊断并修订错误或功能缺口。

### 启用用户反馈
{: #enable_user_feedback}

完成以下步骤，使移动应用程序能够捕获用户反馈。

#### 检测应用程序
{: #instrument_app}

* 检测移动应用程序以进入反馈方式。调用 API `Analytics.triggerFeedbackMode();` 可调用反馈方式。<!--For more information, refer to the documentation [here](instrument_an_app.html)-->.
* 可以对任何应用程序事件（如按钮、菜单操作或手势）调用此 API。

#### 接收用户反馈
{: #receive_feedback}

* 通过触发在其中检测反馈的应用程序操作，应用程序的用户和测试者可以切换到反馈方式。
* 在反馈方式下，可以收集丰富的上下文反馈和截屏，并将其发送给 Mobile Analytics。

#### 分析用户反馈
{: #analyze_feedback}

* Mobile Analytics 收到移动应用程序发送的丰富上下文反馈并进行合并。
* 登录到 Mobile Analytics 控制台，然后选择**用户反馈**选项以查看反馈。
* 应用程序所有者可以复查反馈，添加注释以及使用复查状态来标记反馈。注释通常可以是为了处理反馈而创建的计划操作（例如，Git Issues 的链接），或者注释可以是说明为什么不需要根据反馈执行任何操作的陈述。
* 可以使用复查状态将反馈分类到其中一个不同的复查状态选项下，从而高效地管理反馈。

