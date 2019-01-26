---
title: 招待メッセージの構成
description: invitedUserMessageInfo オブジェクトでは、招待メッセージを構成できます。
localization_priority: Normal
ms.openlocfilehash: 43a5b8cf60ff30d7d7c19736cc78f44eb40fec64
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577376"
---
# <a name="configuring-the-invitation-message"></a>招待メッセージの構成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

invitedUserMessageInfo オブジェクトでは、[招待](../resources/invitation.md)メッセージを構成できます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ccRecipients| [受信者](../resources/recipient.md)のコレクション |招待メッセージの送信先にする必要がある追加の受信者。現在、サポートされている追加の受信者は 1 人のみです。|
|customizedMessageBody|String|既定のメッセージを使用しない場合に送信するカスタマイズされたメッセージ本文。|
|messageLanguage|String|既定のメッセージを送信する言語。customizedMessageBody が指定されている場合、このプロパティは無視され、メッセージは ustomizedMessageBody を使用して送信されます。言語書式は ISO 639 である必要があります。既定では ja-JP です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "#microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitedusermessageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
