---
title: timeZoneBase リソースの種類
description: タイム ゾーンの基本的な表現です。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4ddc8b01f494ee861d3ab50583dc12ea4c68c623
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033573"
---
# <a name="timezonebase-resource-type"></a>timeZoneBase リソースの種類

タイム ゾーンの基本的な表現です。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| name | string | タイム ゾーンの名前。 標準的なタイム ゾーンの名前 ("ハワイ アリューシャン標準時" など) を使用することも、カスタム タイム ゾーンとして "カスタム タイム ゾーン" という名前を指定することもできます。 |


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
