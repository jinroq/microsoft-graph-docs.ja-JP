---
title: plan/バケットリソースの種類
description: ) Office 365 のプラン内のタスク。 これはプランに含まれており、plan グループのタスクのコレクションを持つことができます。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 8cfc25e5554b20d4f808c8929b53549f4c44d7a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462299"
---
# <a name="plannerbucket-resource-type"></a>plan/バケットリソースの種類

**plan**は、Office 365 のプランに含まれるタスクのバケット (または "ユーザー設定列") を表します。 これは[プラン](plannerplan.md)に含まれており、plan グループの[タスク](plannertask.md)のコレクションを持つことができます。



## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |**プラン**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[plannerTasks を一覧表示する](../api/plannerbucket-list-tasks.md) |[plannerTask](plannertask.md) コレクション| プランを取得する**タスク**オブジェクトコレクション。|
|[Create](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | 新しい**プラン**のオブジェクトを作成します。 |
|[Update](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |**プラン**オブジェクトを更新します。 |
|[削除する](../api/plannerbucket-delete.md) | なし |**プラン**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 バケットの ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。|
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
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
