---
title: プランユーザーリソースの種類
description: '**plan ユーザー**リソースは、ユーザーの Planner リソースへのアクセスを提供します。 使用可能なプロパティは含まれていません。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549826"
---
# <a name="planneruser-resource-type"></a>プランユーザーリソースの種類

**plan ユーザー**リソースは、[ユーザー](user.md)の Planner リソースへのアクセスを提供します。 使用可能なプロパティは含まれていません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[計画を一覧表示する](../api/planneruser-list-plans.md) |[plannerPlan](plannerplan.md) コレクション| **プラン**オブジェクトのコレクションを取得します。|
|[タスクを一覧表示する](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) コレクション| プランを取得する**タスク**オブジェクトコレクション。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 プラン enruser の識別子|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|plans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用。 Null 許容型。 ユーザーに割り当てられた担当者の[タスク](plannertask.md)を返します。|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用。 Null 許容型。 ユーザーと共有している[プラン](plannerplan.md)を返します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
