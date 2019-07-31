---
title: mediaInfo リソースの種類
description: プロンプトのアクションで使用されるメディア情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6a5e5677cb479839449a5e82323729b68201791a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966870"
---
# <a name="mediainfo-resource-type"></a>mediaInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロンプトのアクションで使用されるメディア情報。

## <a name="properties"></a>プロパティ
| プロパティ       | 型    | 説明                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | 省略可能。リソースを一意に識別するために使用されます。 渡された場合、プロンプト uri はこの resourceId に対してキーとしてキャッシュされます。 |
| uri            | String  | 再生するプロンプトへのパス。 現時点では、Wave ファイル (.wav) 形式のみで、16000 (16KHz) のサンプリングレートを持つ16ビットのサンプルのみがサポートされています。 |


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
