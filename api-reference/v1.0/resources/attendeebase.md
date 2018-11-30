---
title: attendeeBase リソースの種類
description: 出席者の種類です。
ms.openlocfilehash: 6995ac94a600a60313ef26208b441c6ef6fdf001
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022828"
---
# <a name="attendeebase-resource-type"></a>attendeeBase リソースの種類

出席者の種類です。

[recipient](recipient.md) から派生します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|type|attendeeType| 出席者の種類です。 可能な値: `required`、 `optional`、 `resource`。 現在、出席者が人間の場合は、 [findMeetingTimes](../api/user-findmeetingtimes.md)は一切の人では、`Required`型です。|
|emailAddress|[emailAddress](emailaddress.md)|参加者の名前と SMTP アドレスが含まれます。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
