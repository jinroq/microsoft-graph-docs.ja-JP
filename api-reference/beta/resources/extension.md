---
title: 拡張子リソースの種類
description: OData v4 のオープン型 openTypeExtension をサポートする抽象型。
localization_priority: Normal
ms.openlocfilehash: b261ceeff4639b8a602edbb411b34ab19d46ea8e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542637"
---
# <a name="extension-resource-type"></a>拡張子リソースの種類

OData v4 のオープン型 [openTypeExtension](opentypeextension.md) をサポートする抽象型。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
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
|id|String| 読み取り専用です。|

## <a name="relationships"></a>関係
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
