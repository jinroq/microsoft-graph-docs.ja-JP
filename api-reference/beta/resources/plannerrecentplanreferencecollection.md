---
title: plannerRecentPlanReferenceCollection リソースの種類
description: '**plannerRecentPlanReferenceCollection**リソースは、ユーザーが最近参照したプランへの参照のコレクションを表します。 このリソースはオープンタイプで、プランのユーザーオブジェクトの一部です。 プロパティ名は、対応するプランの ID です。 プロパティと値のペアの値は、plannerRecentPlanReference オブジェクトです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a2b2607f8b5cf3dbd91e69ab71a737037cbd0a94
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344348"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>plannerRecentPlanReferenceCollection リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerRecentPlanReferenceCollection**リソースは、ユーザーが最近参照したプランへの参照のコレクションを表します。 このリソースはオープンタイプで、[プランのユーザー](planneruser.md)オブジェクトの一部です。 プロパティ名は、対応するプランの ID です。 プロパティと値のペアの値は、 [plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトです。
このコレクションに新しい参照を追加すると、コレクションのサイズが事前に定義された最大値を超えると、最も古いエントリが自動的に削除されます。


## <a name="properties"></a>プロパティ
このオープン型のプロパティを定義できます。 プロパティ名は、 `id` plan リソース[](plannerplan.md)およびその値が[plannerRecentPlanReference](plannerrecentplanreference.md)オブジェクトである必要があることを示す値です。 [お気に入り] の一覧から項目を削除するには、プロパティの値`null`をに設定します。


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
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
