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

# 在主控台上視覺化見解
{: #visualize_insights_on_console}

從「MobileFirst Analytics 主控台」中，您可以檢視及配置 Analytics 報告、管理警示，以及檢視用戶端日誌。按一下左導覽中的**分析主控台**，以從「Mobile Foundation 作業主控台」中啟動「Analytics 主控台」。

即會啟動「Analytics 主控台」，並出現預設儀表板。如果用戶端應用程式已將日誌及分析資料傳送至伺服器，則會建立並顯示相關報告。從儀表板中，您可以檢閱所收集的分析資料。此分析資料可能與應用程式損毀、應用程式階段作業及伺服器處理時間相關。此外，您可以建立自訂圖表以及管理警示。

除了行動分析的摘要視圖之外，分析特性還能夠針對用戶端日誌、已擷取之用戶端損毀資料和您透過用戶端 API 函數呼叫（會提供給 Mobile Analytics）明確提供之任何額外資料，執行原始搜尋。

## 監視應用程式資料
{: #monitoring_app_data}

Mobile Analytics 可提供行動應用程式的監視及分析。您可以使用 Mobile Analytics Client SDK 來記錄應用程式日誌以及監視資料。開發人員可以控制何時將此資料傳送至「Mobile Analytics 服務」。將資料遞送至 Mobile Analytics 時，您可以使用 Mobile Analytics 主控台來取得行動應用程式、裝置及應用程式日誌的分析見解。

可衍生的部分見解：

**預先定義的度量值**

您可以使用預先定義的度量值來回答下列這類問題：
* 我有多少位新使用者？
* 有多少人正活躍地使用我的應用程式？
* 他人使用我的應用程式的頻率為何？
* 他人在什麼時間使用我的應用程式？
* 我的使用者喜歡哪些裝置模型？
* 我應該何時淘汰支援舊式作業系統？
* 哪些應用程式發生效能問題？

**自訂事件**

藉由新增自己的自訂事件，您可以回答下列這類問題：
* 最常使用及最少使用的特性為何？
* 使用者在哪裡進入及離開我的應用程式？
* 使用者最常檢視的活動為何？
* 使用者是否在應用程式中完成工作流程（例如，轉換通道）？

## 可視覺化的報告：使用者
{: #reports_visualized_users}

此報告顯示的圖表顯示在指定的日期範圍內已使用應用程式的作用中使用者數目。報告也會顯示新使用者數目，而新使用者是在指定日期範圍內第一次使用應用程式的唯一使用者。可以根據應用程式名稱、作業系統或作業系統版本來過濾圖表。

## 可視覺化的報告：階段作業
{: #reports_visualized_sessions}

此報告顯示的圖表顯示指定日期範圍內的「應用程式階段作業」。將應用程式帶到裝置前景時，會記錄階段作業。可以根據應用程式名稱、作業系統或作業系統版本來過濾圖表。

## 可視覺化的報告：網路要求
{: #reports_visualized_network_requests}

在 Mobile Analytics 主控台中，針對您的應用程式視覺化網路要求資料。

資料可供下列測量使用：

**往返時間** - 定義應用程式提出網路要求所需的時間長度（以毫秒為測量單位）。**要求計數** - 顯示應用程式提出網路要求的頻率。資料也顯示為平均值。可以根據應用程式名稱、作業系統或作業系統版本來過濾圖表。

## 可視覺化的報告：損毀
{: #reports_visualized_crashes}

您可以在 Mobile Analytics 主控台中檢視應用程式損毀的相關資訊，以更適當地監視應用程式並進行疑難排解。

在「損毀」頁面上，**損毀概觀**表格會顯示下列資料直欄：

**應用程式**：應用程式名稱<br/>
**損毀**：該應用程式的損毀總數<br/>
**使用總計**：使用者開啟及關閉該應用程式的總次數<br/>
**損毀率**：每次使用的損毀百分比<br/>
您可以在「損毀」表格中快速查看應用程式損毀的相關資訊。「損毀」長條圖會顯示一段時間內損毀的直方圖。<br/>

您可以使用兩種方式來顯示損毀資料：

1.  顯示損毀率：一段時間的損毀率
2.  顯示損毀總計：一段時間的損毀總計

## 可視覺化的報告：疑難排解
{: #reports_visualized_troubleshooting}

Mobile Analytics 主控台中的**疑難排解**頁面會使用**損毀摘要**表格來提供應用程式損毀的精細視圖。

**損毀摘要**表格可進行排序，而且包括下列資料直欄：

* 損毀數
* 裝置數
* 前次損毀
* 應用程式
* OS
* 訊息

按一下任何項目旁的 + 圖示來顯示**損毀詳細資料**表格，其中包括下列直欄：

* 損毀時間
* 應用程式版本
* OS 版本
* 裝置型號
* 裝置 ID
* 下載：下載導致損毀的日誌的鏈結

展開**損毀詳細資料**表格中的任何項目，以取得更多詳細資料（包括堆疊追蹤）。

**損毀摘要**表格的資料是透過查詢嚴重層次應用程式日誌移入的。如果您的應用程式未收集嚴重應用程式日誌，則沒有任何可用資料。
{: note}


## 可視覺化的報告：使用者意見
{: #reports_visualized_userfeedback}

「使用者意見」提供用於使用 Mobile Analytics 分析應用程式內意見。使用此 Mobile Analytics 特性 -
* **使用者及測試人員**可以在執行及使用應用程式時，記錄並傳送應用程式的意見及錯誤報告。
* **應用程式擁有者**可透過此環境定義豐富的使用者意見，更深入瞭解應用程式的使用者體驗。
* 不過，**開發人員**會接收精確的應用程式環境定義，以診斷並修正錯誤或特性間隙。

### 啟用使用者意見
{: #enable_user_feedback}

請完成下列步驟，讓行動應用程式擷取使用者意見。

#### 檢測應用程式
{: #instrument_app}

* 檢測行動應用程式，以進入意見模式。呼叫 API `Analytics.triggerFeedbackMode();`，以呼叫意見模式。<!--For more information, refer to the documentation [here](instrument_an_app.html)-->.
* 您可以對任何應用程式事件（例如按鈕、功能表動作或手勢）呼叫 API。

#### 接收使用者意見
{: #receive_feedback}

* 應用程式的使用者及測試人員可以藉由觸發要針對意見檢測的應用程式動作，來切換至意見模式。
* 在意見模式內，可以收集豐富環境定義意見及畫面擷取，並將其傳送至 Mobile Analytics。

#### 分析使用者意見
{: #analyze_feedback}

* Mobile Analytics 會接收及合併從行動應用程式傳出的豐富環境定義意見。
* 登入 Mobile Analytics 主控台，然後選取**使用者意見**選項來檢視意見。
* 應用程式擁有者可以檢閱意見、新增註解，並使用檢閱狀態來標記意見。註解通常可以是建立以處理意見的規劃動作（例如 Git 問題的鏈結），註解也可以是證明不需要對意見採取任何動作之原因的陳述。
* 檢閱狀態可以用來有效率地管理意見，方法是將它們分類為其中一個不同的檢閱狀態選項。

