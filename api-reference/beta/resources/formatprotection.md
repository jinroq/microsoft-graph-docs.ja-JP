---
title: FormatProtection リソースの種類
description: 範囲オブジェクトの書式保護を表します。
localization_priority: Normal
ms.openlocfilehash: 0b4add2e30a1e475adcb162903f771ce760f9285
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805622"
---
# <a name="formatprotection-resource-type"></a>FormatProtection リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

範囲オブジェクトの書式保護を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[FormatProtection を取得する](../api/formatprotection-get.md) | [FormatProtection](formatprotection.md) |formatProtection オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/formatprotection-update.md) | [FormatProtection](formatprotection.md)  |FormatProtection オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|formulaHidden|ブール値|Excel が範囲内のセルの数式を非表示にするかどうかを示します。null 値は、範囲全体に一様な数式非表示設定がないことを表します。|
|locked|ブール値|Excel がオブジェクト内のセルをロックするかどうかを示します。null 値は、範囲全体に一様なロック設定がないことを表します。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
