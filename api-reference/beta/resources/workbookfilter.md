---
title: workbookFilter リソースの種類
description: テーブルの列のフィルター処理を管理します。
localization_priority: Normal
ms.openlocfilehash: 79ded0bfca0ace3b2d7c1bcdb4cd8dd2696802a4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348906"
---
# <a name="workbookfilter-resource-type"></a>workbookFilter リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テーブルの列のフィルター処理を管理します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Apply](../api/filter-apply.md)|なし|指定した列に指定されたフィルター条件を適用します。|
|[Clear](../api/filter-clear.md)|なし|指定した列のフィルターをクリアします。|

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|criteria|[workbookFilterCriteria](workbookfiltercriteria.md)|指定した列に現在適用されているフィルターです。 読み取り専用です。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
    "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
