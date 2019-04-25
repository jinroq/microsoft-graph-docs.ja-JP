---
title: プラン/お気に入りプラン referencecollection リソースの種類
description: " この値は、\"プラン参照\" オブジェクトを示します。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c473d4101a1247420e641b532ea04dfbc1a26d2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572627"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>プラン/お気に入りプラン referencecollection リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plan**は、ユーザーによってお気に入りとしてマークされているプランへの参照のコレクションを表します。 このリソースはオープンタイプで、[プランのユーザー](planneruser.md)オブジェクトの一部です。 プロパティと値のペアのプロパティ名は、対応するプランの ID です。この値は、"[プラン参照](plannerfavoriteplanreference.md)" オブジェクトを示します。


## <a name="properties"></a>プロパティ
このオープン型のプロパティを定義できます。 プロパティ名は`id` 、plan リソースとその値を[プラン](plannerplan.md)にする必要が[](plannerfavoriteplanreference.md)あります。 [お気に入り] の一覧から項目を削除するには、プロパティの値`null`をに設定します。


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
