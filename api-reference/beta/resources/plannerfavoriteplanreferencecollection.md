---
title: plannerFavoritePlanReferenceCollection リソースの種類
description: " 値は、plannerFavoritePlanReference オブジェクトです。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 333d7f354f056945de52687eefc8bb862ac48e75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967113"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>plannerFavoritePlanReferenceCollection リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**PlannerFavoritePlanReferenceCollection**リソースでは、ユーザーがお気に入りとしてマークされている計画への参照のコレクションを表します。 このリソースは、オープン型であり、 [plannerUser](planneruser.md)オブジェクトの一部であります。 プロパティ名、プロパティ値のペアでは、対応する計画の ID をします。値は、 [plannerFavoritePlanReference](plannerfavoriteplanreference.md)オブジェクトです。


## <a name="properties"></a>プロパティ
このオープン型のプロパティを定義することができます。 プロパティ名は、 `id` [plannerPlan](plannerplan.md)リソースの値とその値は、 [plannerFavoritePlanReference](plannerfavoriteplanreference.md)オブジェクトをする必要があります。 お気に入りの一覧で項目を削除するのにはプロパティの値を設定します`null`。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
}-->

```json
{
  "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586866870001551087",
    "planTitle": "Customer reviews"
  },
  "uZWtCtli30CGoWLIWSat1mQAC0ai": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586848705198093378",
    "planTitle": "Order Management (December 2017)"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
