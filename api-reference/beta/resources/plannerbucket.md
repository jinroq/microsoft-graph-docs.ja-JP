---
title: Plan/バケットリソースの種類
description: ) Office 365 のプラン内のタスク。 これはプランに含まれており、plan グループのタスクのコレクションを持つことができます。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: eed92a62fed8077d2b7ee541feac7e0fa5c73483
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966010"
---
# <a name="plannerbucket-resource-type"></a>Plan/バケットリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Plan**は、Office 365 のプランに含まれるタスクのバケット (または "ユーザー設定列") を表します。 これは[プラン](plannerplan.md)に含まれており、plan グループの[タスク](plannertask.md)のコレクションを持つことができます。



## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |**プラン**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[plannerTasks を一覧表示する](../api/plannerbucket-list-tasks.md) |[plannerTask](plannertask.md) コレクション| **plannerTask** オブジェクト コレクションを取得します。|
|[Create](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | 新しい**プラン**のオブジェクトを作成します。 |
|[Update](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |**プラン**オブジェクトを更新します。 |
|[Delete](../api/plannerbucket-delete.md) | None |**プラン**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|文字列| 読み取り専用。 バケットの ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。|
|name|String|バケットの名前。|
|orderHint|String|リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|
|planId|String|バケットが属している計画 ID。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。 Null 許容型。 バケット内のタスクのコレクション。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
