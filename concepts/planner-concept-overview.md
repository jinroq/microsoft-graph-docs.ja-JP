---
title: Planner のタスクおよびプラン API の概要
description: Planner は、チームが作業を組織するためのシンプルかつビジュアルな手段を提供します。 顧客は Planner を使用することにより、プランを作成したり、タスクを組織して割り当てたり、進捗状況を共有したり、コンテンツに対して共同作業をしたりできます。  Planner は、タスク ボード、グラフ ページ、スケジュール ビューなどのインタラクティブなエクスペリエンスを提供し、Office 365 を通じた機能統合を実現します。
ms.openlocfilehash: c2accfb200c9c55416872b5e5e240583db5396ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092509"
---
# <a name="planner-tasks-and-plans-api-overview"></a>Planner のタスクおよびプラン API の概要
Planner は、チームが作業を組織するためのシンプルかつビジュアルな手段を提供します。 顧客は Planner を使用することにより、プランを作成したり、タスクを組織して割り当てたり、進捗状況を共有したり、コンテンツに対して共同作業をしたりできます。  Planner は、タスク ボード、グラフ ページ、スケジュール ビューなどのインタラクティブなエクスペリエンスを提供し、Office 365 を通じた機能統合を実現します。

**Office 365 Planner タスク ボード**

![Office 365 Planner タスク ボードのスクリーン ショット](images/plannerboard.png "Planner ボードの画像")


## <a name="why-integrate-with-planner-tasks"></a>Planner タスクを統合する理由
Planner は、Office 365 でのコラボレーション エクスペリエンスのためのタスク追跡機能を提供します。 エンド ユーザーのチームやグループのためのタスク追跡機能や作業を組織する機能が必要な場合、Planner が最適です。 Planner 統合は、Office 365 でコラボレーションする何百万というユーザーに達するのに役立ちます。 

### <a name="organize-your-teams-work"></a>チームの作業を組織する
Planner は、チームを立ち上げ、[タスクを作成し](/graph/api/planner-post-tasks?view=graph-rest-1.0)、それをチームの他のメンバーに割り当てるための共有スペースを提供します。 Planner を利用すれば、誰が何をしているのかを容易に把握でき、順調に事が進んでいるかどうかを確認できます。期限、進捗状況、説明などの追加情報によりタスクを更新し、カスタマイズ可能なバケットとカテゴリ ラベルによりタスクを詳細に組織することができます。   

### <a name="collaborate-across-office-365"></a>Office 365 を通じた共同作業
Planner は、Office 365 を通じてコラボレーション エクスペリエンスに統合されています。 Planner の Web およびモバイル クライアントに加えて、ユーザーは Planner のプランやタスクを SharePoint および Microsoft Teams から表示したり更新したりできます。  

Planner 自体でも Microsoft Graph および Office 365 のグループ サービスが利用されています。 アップロードして Planner タスクに添付するファイルは、SharePoint に保存されます。 Planner のコメントは、Outlook のグループ会話に基づいています。

<!-- Add image
Note: Put an image here showing the relationship between Planner and other things
-->

### <a name="automate-the-creation-of-plans-and-tasks"></a>プランおよびタスクの作成の自動化
繰り返されるプロセスやプロジェクト タイプの作業をしていますか。 Planner API を使用することにより、プランやタスク リストの作成を自動化できます。  
 
## <a name="top-planner-api-tasks"></a>Planner API のトップ タスク

|操作|URL|
|:--------|:--|
|グループの[プラン](/graph/api/resources/plannerplan?view=graph-rest-beta)をすべて表示|GET [https://graph.microsoft.com/v1.0/groups/{id}/planner/plans](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|プラン内の[タスク](/graph/api/resources/plannertask?view=graph-rest-beta)を表示|GET [https://graph.microsoft.com/v1.0/planner/plans/{id}/tasks](https://developer.microsoft.com/graph/graph-explorer?request=planner/plans/{id}/tasks&version=v1.0)|
|複数のプランを通じて自分に割り当てられている[マイ タスク](/graph/api/planneruser-list-tasks?view=graph-rest-beta)をすべて表示|GET [https://graph.microsoft.com/v1.0/me/planner/tasks/](https://developer.microsoft.com/graph/graph-explorer?request=me/planner/tasks/&version=v1.0)|
|[新しいタスクを作成](/graph/api/planner-post-tasks?view=graph-rest-1.0)|POST [https://graph.microsoft.com/v1.0/planner/tasks](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[タスクを更新](/graph/api/plannertask-update?view=graph-rest-1.0)|PATCH [https://graph.microsoft.com/v1.0/planner/tasks/{task-id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[タスクを削除](/graph/api/plannertask-delete?view=graph-rest-1.0)|DELETE [https://graph.microsoft.com/v1.0/planner/tasks/{id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の Planner API](/graph/api/resources/planner-overview?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の Planner API](/graph/api/resources/planner-overview?view=graph-rest-beta)


## <a name="next-steps"></a>次のステップ

- [Planner API を使用する](/graph/api/resources/planner-overview?view=graph-rest-1.0)
- [プランを操作する](/graph/api/resources/planner-overview?view=graph-rest-1.0#plans)
- [タスクを操作する](/graph/api/resources/planner-overview?view=graph-rest-1.0#tasks)
