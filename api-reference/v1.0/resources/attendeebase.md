---
title: attendeeBase リソースの種類
description: 出席者の種類です。
localization_priority: Normal
ms.openlocfilehash: d009ef6a58c63017addf8b8a1bdecc1974abbff3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569355"
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
|type|attendeeType| 出席者の種類です。 使用可能な値: `required`、`optional`、`resource`。 現時点では、出席者が 1 人である場合、[findMeetingTimes](../api/user-findmeetingtimes.md) では常にその人は `Required` 型と見なされます。|
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
