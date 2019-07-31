---
title: responseStatus リソースの種類
description: 会議出席依頼の応答状態です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a28987d48aa7861a883ac93f53aca63ecaeab9d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965384"
---
# <a name="responsestatus-resource-type"></a>responseStatus リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議出席依頼の応答状態です。

## <a name="properties"></a>プロパティ

| プロパティ | 型           | 説明 |
|:---------|:---------------|:------------|
| response | String         | 応答の種類。 可能な値は `None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded` です。
| time     | DateTimeOffset | 応答が返された日時。ISO 8601 形式を使って表され、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
