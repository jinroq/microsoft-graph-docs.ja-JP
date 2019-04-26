---
title: プランワークプランの詳細リソースの種類
description: "\"plan/プランの**詳細**\" リソースは、プランに関する追加情報を表します。 各 plan オブジェクトには details オブジェクトがあります。"
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 51bc28e93f7978fb080969de413db4e804918f6d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344404"
---
# <a name="plannerplandetails-resource-type"></a>プランワークプランの詳細リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

"plan/プランの**詳細**" リソースは、プランに関する追加情報を表します。 各[plan](plannerplan.md)オブジェクトには details オブジェクトがあります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |**plan**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |"plan/プランの**詳細**" オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト|
|id|String| 読み取り専用です。 プランの詳細の ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。|
|sharedWith|[plannerUserIds](planneruserids.md)|このプランで共有される一連のユーザー id。 Office 365 グループを使用している場合は、グループのメンバーシップを管理するグループの API を使用して、グループ[の](group.md)計画を共有します。 グループの既存のメンバーをこのコレクションに追加することもできますが、グループが所有しているプランにアクセスするために必要ではありません。 |
|contextdetails|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)|読み取り専用です。 プランに関連付けられている追加情報のコレクション。 plan の[プラン](plannerplan.md)コンテナーに対して定義された[コンテキスト](plannerplancontext.md)エントリ。 |

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
