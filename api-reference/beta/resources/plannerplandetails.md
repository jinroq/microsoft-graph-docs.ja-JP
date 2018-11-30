---
title: plannerPlanDetails リソースの種類
description: '**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 plan オブジェクトには詳細オブジェクトがあります。'
ms.openlocfilehash: 1cce5727666bca705da67fccd1a3edf370c68127
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073090"
---
# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 [plan](plannerplan.md) オブジェクトには詳細オブジェクトがあります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |プロパティと、 **plannerPlanDetails**オブジェクトの関係を参照してください。|
|[Update](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |**PlannerPlanDetails**オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト|
|id|String| 読み取り専用。 計画の ID です。 28 の文字、大文字小文字を区別することをお勧めします。 サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。|
|sharedWith|[plannerUserIds](planneruserids.md)|一連のユーザーと共有は、この計画の Id。 Office 365 のグループを使用する場合は、[グループ](group.md)の計画を共有するグループ メンバーシップを管理するグループの API を使用します。 グループによって所有されているプランにアクセスするために必要はありませんが、このコレクションにグループの既存のメンバーを追加できます。 |
|contextDetails|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)|読み取り専用。 [PlannerPlan](plannerplan.md)コンテナーに定義されている[plannerPlanContext](plannerplancontext.md)のエントリに関連付けられているその他の情報のコレクションです。 |

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記
リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
