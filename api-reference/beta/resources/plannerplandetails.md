---
title: プランワークプランの詳細リソースの種類
description: "\"Plan/プランの**詳細**\" リソースは、プランに関する追加情報を表します。 各 plan オブジェクトには details オブジェクトがあります。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 61296138f1477219e85ae7fd372102b8c7fd3a47
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965888"
---
# <a name="plannerplandetails-resource-type"></a>プランワークプランの詳細リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

"Plan/プランの**詳細**" リソースは、プランに関する追加情報を表します。 各[plan](plannerplan.md)オブジェクトには details オブジェクトがあります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |**Plan**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |"Plan/プランの**詳細**" オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト|
|id|String| 読み取り専用です。 プランの詳細の ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。|
|sharedWith|[plannerUserIds](planneruserids.md)|このプランで共有される一連のユーザー Id。 Office 365 グループを使用している場合は、グループのメンバーシップを管理するグループの API を使用して、グループ[の](group.md)計画を共有します。 グループの既存のメンバーをこのコレクションに追加することもできますが、グループが所有しているプランにアクセスするために必要ではありません。 |
|contextDetails|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)|読み取り専用です。 プランに関連付けられている追加情報のコレクション。 plan の[プラン](plannerplan.md)コンテナーに対して定義された[コンテキスト](plannerplancontext.md)エントリ。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
