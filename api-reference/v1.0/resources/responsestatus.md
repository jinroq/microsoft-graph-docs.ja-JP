---
title: responseStatus リソースの種類
description: 会議出席依頼の応答状態です。
localization_priority: Normal
ms.openlocfilehash: 110b0eb158043b9573deb3e3ced792119bfa91a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579283"
---
# <a name="responsestatus-resource-type"></a>responseStatus リソースの種類

会議出席依頼の応答状態です。

## <a name="properties"></a>プロパティ

| プロパティ | 型           | 説明 |
|:---------|:---------------|:------------|
| response | responseType   | 応答の種類。 使用可能な値は`None`、 `Organizer`、 `TentativelyAccepted` `Accepted` `Declined`、、、 `NotResponded`、です。
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
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
