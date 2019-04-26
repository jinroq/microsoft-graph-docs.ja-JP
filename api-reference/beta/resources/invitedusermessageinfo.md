---
title: 招待メッセージの構成
description: invitedUserMessageInfo オブジェクトを使用すると、招待メッセージを構成できます。
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569971"
---
# <a name="configuring-the-invitation-message"></a>招待メッセージの構成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

invitedUserMessageInfo オブジェクトを使用すると、[招待](invitation.md)メッセージを構成できます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ccRecipients|[受信者](recipient.md)|その他の受信者に招待メッセージを送信する必要があります。 現時点では、1つの追加の受信者のみがサポートされています。|
|customizedmessagebody|String|既定のメッセージを必要としない場合に送信する、カスタマイズされたメッセージ本文。|
|messageLanguage|String|既定のメッセージを送信する言語を指定します。 customizedmessagebody が指定されている場合、このプロパティは無視され、customizedmessagebody を使用してメッセージが送信されます。 言語の形式は ISO 639 である必要があります。 既定値は en-us です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
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
