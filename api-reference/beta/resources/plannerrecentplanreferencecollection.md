---
title: plannerRecentPlanReferenceCollection リソースの種類
description: '**PlannerRecentPlanReferenceCollection**リソースでは、ユーザーが最近表示されたプランへの参照のコレクションを表します。 このリソースは、オープン型であり、plannerUser オブジェクトの一部であります。 プロパティ名は、対応する計画の ID です。 プロパティと値のペアの値は、plannerRecentPlanReference オブジェクトです。'
ms.openlocfilehash: b22f7367a1826c95889b63a6884885ce49497c33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074329"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>plannerRecentPlanReferenceCollection リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**PlannerRecentPlanReferenceCollection**リソースでは、ユーザーが最近表示されたプランへの参照のコレクションを表します。 このリソースは、オープン型であり、 [plannerUser](planneruser.md)オブジェクトの一部であります。 プロパティ名は、対応する計画の ID です。 プロパティと値のペアの値は、 [plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトです。
このコレクションに新しい参照を追加するがコレクションのサイズが事前に定義された最大値を超えたときに自動的に最も古いエントリを削除します。


## <a name="properties"></a>プロパティ
このオープン型のプロパティを定義することができます。 プロパティ名は、 `id` [plannerPlan](plannerplan.md)リソースの値とその値は、 [plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトをする必要があります。 お気に入りの一覧で項目を削除するのにはプロパティの値を設定します`null`。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
}-->

```json
{
  "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-02T22:49:46.155Z",
    "planTitle": "Purchase Workflow"
  },
  "iKNMHkk3vEWpSF7F7iZWIGQAAMMw": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-03T21:59:28.975Z",
    "planTitle": "New Year's Office Party"
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
