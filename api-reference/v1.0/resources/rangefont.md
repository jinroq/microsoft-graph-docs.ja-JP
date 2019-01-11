---
title: RangeFont リソースの種類
description: このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
ms.openlocfilehash: 32bbd29706966c4c4b15f038ebdbb872b1dd8193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856582"
---
# <a name="rangefont-resource-type"></a>RangeFont リソースの種類

このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[RangeFont を取得する](../api/rangefont-get.md) | [WorkbookRangeFont](rangefont.md) |rangeFont オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/rangefont-update.md) | [WorkbookRangeFont](rangefont.md)   |RangeFont オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|bold|ブール値|フォントの太字の状態を表します。|
|color|文字列|テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。|
|italic|ブール値|フォントの斜体の状態を表します。|
|name|文字列|フォント名 (例: "Calibri")|
|size|double|フォント サイズ|
|underline|文字列|フォントに適用する下線の種類です。 可能な値: `None`、 `Single`、 `Double`、 `SingleAccountant`、 `DoubleAccountant`。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
