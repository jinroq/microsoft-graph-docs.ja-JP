---
title: planner リソースの種類
description: '**planner**リソースは、planner オブジェクトモデルのエントリポイントです。 シングルトン**プランナー**リソースを返します。  使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f6d25238436b79dec0397df1d005e67e6b17239a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462278"
---
# <a name="planner-resource-type"></a>planner リソースの種類

**planner**リソースは、planner オブジェクトモデルのエントリポイントです。 シングルトン**プランナー**リソースを返します。  使用可能なプロパティは含まれていません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| バケットコレクションへの投稿により、新しい**プラン**を作成します。|
|[Create plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| プランコレクションへの投稿によって、新しい**プラン**を作成します。|
|[Create plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| タスクコレクションへの投稿によって、新しい**プラン**を作成します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|buckets|[プラン | バケット](plannerbucket.md)コレクション| 読み取り専用です。 Null 許容型。 指定したバケットのコレクションを返します。|
|plans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。 Null 許容型。 指定したプランのコレクションを返します。|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。 Null 許容型。 指定したタスクのコレクションを返します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a>例

**プランナー**リソースは、グラフのルートにあります。

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
