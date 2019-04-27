---
title: workbookApplication リソースの種類
description: ブックを管理する Excel workbookApplication を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 3db8c640ebb2fd36a0902563c28a3ec51bfa99d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348880"
---
# <a name="workbookapplication-resource-type"></a>workbookApplication リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ブックを管理する Excel アプリケーションを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookApplication を取得する](../api/workbookapplication-get.md) | [workbookApplication](workbookapplication.md) |workbookApplication オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Calculate](../api/workbookapplication-calculate.md)|なし|Excel で現在開いているすべてのブックを再計算します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|calculationMode|string|ブックで使用されている計算モードを返します。 可能な値は、`Automatic`、`AutomaticExceptTables`、`Manual` です。 読み取り専用です。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
