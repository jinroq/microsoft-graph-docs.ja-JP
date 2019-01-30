---
title: automaticRepliesSetting リソースの種類
description: 'メッセージを受信したメールの送信者に自動的に通知する設定を構成します '
localization_priority: Normal
ms.openlocfilehash: 5ff16aa93042e0d66063cb62de7a8dcdf870c892
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641254"
---
# <a name="automaticrepliessetting-resource-type"></a>automaticRepliesSetting リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。たとえば、サインイン ユーザーが電子メールに返信できないことを通知する自動返信などです。 


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|externalAudience|String| **Status** が `AlwaysEnabled` または `Scheduled` の場合に、**ExternalReplyMessage** を受信する、サインイン ユーザーの組織外の一連の対象ユーザー。可能な値は、`none`、`contactsOnly`、`all` です。|
|externalReplyMessage|string|**Status** が `AlwaysEnabled` または `Scheduled` の場合、指定の外部対象ユーザーに送信される自動応答。|
|internalReplyMessage|string|**Status** が `AlwaysEnabled` または `Scheduled` の場合、サインイン ユーザーの組織内の対象ユーザーに送信される自動応答。 |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|**Status** が `Scheduled` に設定されている場合に、自動応答を終了する日時。 |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|**Status** が `Scheduled` に設定されている場合に、自動応答を開始する日時。|
|status|String|自動応答の構成状態。可能な値は、`disabled`、`alwaysEnabled`、`scheduled` です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliessetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
