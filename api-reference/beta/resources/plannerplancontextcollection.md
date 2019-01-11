---
title: plannerPlanContextCollection リソースの種類
description: '**PlannerPlanContextCollection**リソースでは、プランがリンクされている外部のコンテキストのコレクションを表します。 このリソースは、オープン型であり、plannerPlan オブジェクトの一部であります。 プロパティと値のペアの値は、plannerPlanContext オブジェクトです。'
localization_priority: Normal
ms.openlocfilehash: 51a09353993a61324f31a03c8ffadd5462cac692
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805454"
---
# <a name="plannerplancontextcollection-resource-type"></a>plannerPlanContextCollection リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。


**PlannerPlanContextCollection**リソースでは、プランがリンクされている外部のコンテキストのコレクションを表します。 このリソースは、オープン型であり、 [plannerPlan](plannerplan.md)オブジェクトの一部であります。 プロパティと値のペアの値は、 [plannerPlanContext](plannerplancontext.md)オブジェクトです。


## <a name="properties"></a>プロパティ
このオープン型のプロパティを定義することができます。 プロパティの値はプロパティ名と外部のコンテキストを表す特徴的な識別子である必要があります。 プロパティの値は、 [plannerPlanContext](plannerplancontext.md)オブジェクトである必要があります。 OData の要件に基づき、オープン型のプロパティ名は次の文字を含めることはできません: `.`、 `:`、 `%`、 `@`。 これらの文字は、URL エンコーディングを使用してエンコードする必要があります。 お気に入りの一覧で項目を削除するのにはプロパティの値を設定します`null`。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
