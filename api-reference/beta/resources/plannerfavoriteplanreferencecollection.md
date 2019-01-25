---
title: plannerFavoritePlanReferenceCollection リソースの種類
description: " 値は、plannerFavoritePlanReference オブジェクトです。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c473d4101a1247420e641b532ea04dfbc1a26d2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519487"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>plannerFavoritePlanReferenceCollection リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
