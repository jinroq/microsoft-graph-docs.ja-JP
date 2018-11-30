---
title: 拡張子リソースの種類
description: OData v4 のオープン型 openTypeExtension をサポートする抽象型。
ms.openlocfilehash: b67c347e44c875ca550465be46eecdff3f845eef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067519"
---
# <a name="extension-resource-type"></a>拡張子リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

OData v4 のオープン型 [openTypeExtension](opentypeextension.md) をサポートする抽象型。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

実際にサポートされるメソッドについては、派生型「[openTypeExtension](opentypeextension.md)」のメソッドを参照してください。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->