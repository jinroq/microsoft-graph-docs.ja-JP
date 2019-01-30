---
title: 参加者リソースの種類
description: イベントの参加者です。 これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。
localization_priority: Normal
ms.openlocfilehash: d50b6756c7d0077ec95f10988d06fa2ff81631fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642878"
---
# <a name="attendee-resource-type"></a>参加者リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

イベントの参加者です。 これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。

[attendeeBase](attendeebase.md) から派生します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|status|[ResponseStatus](responsestatus.md)|イベントに対する参加者からの応答 (なし、承諾、辞退など) と応答が送信された日時。|
|type|String|参加者のタイプは、`required`、`optional`、`resource` です。|
|emailAddress|[emailAddress](emailaddress.md)|参加者の名前と SMTP アドレスが含まれます。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendee.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
