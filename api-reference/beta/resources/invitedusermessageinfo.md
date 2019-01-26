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
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="dfc1b-103">招待メッセージの構成</span><span class="sxs-lookup"><span data-stu-id="dfc1b-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfc1b-104">invitedUserMessageInfo オブジェクトでは、[招待](../resources/invitation.md)メッセージを構成できます。</span><span class="sxs-lookup"><span data-stu-id="dfc1b-104">The invitedUserMessageInfo object allows you to configure the [invitation](../resources/invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="dfc1b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfc1b-105">Properties</span></span>
| <span data-ttu-id="dfc1b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfc1b-106">Property</span></span>     | <span data-ttu-id="dfc1b-107">型</span><span class="sxs-lookup"><span data-stu-id="dfc1b-107">Type</span></span>   |<span data-ttu-id="dfc1b-108">説明</span><span class="sxs-lookup"><span data-stu-id="dfc1b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfc1b-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="dfc1b-109">ccRecipients</span></span>| <span data-ttu-id="dfc1b-110">[受信者](../resources/recipient.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="dfc1b-110">[Recipients](../resources/recipient.md) collection</span></span> |<span data-ttu-id="dfc1b-p101">招待メッセージの送信先にする必要がある追加の受信者。現在、サポートされている追加の受信者は 1 人のみです。</span><span class="sxs-lookup"><span data-stu-id="dfc1b-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="dfc1b-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="dfc1b-113">customizedMessageBody</span></span>|<span data-ttu-id="dfc1b-114">String</span><span class="sxs-lookup"><span data-stu-id="dfc1b-114">String</span></span>|<span data-ttu-id="dfc1b-115">既定のメッセージを使用しない場合に送信するカスタマイズされたメッセージ本文。</span><span class="sxs-lookup"><span data-stu-id="dfc1b-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="dfc1b-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="dfc1b-116">messageLanguage</span></span>|<span data-ttu-id="dfc1b-117">String</span><span class="sxs-lookup"><span data-stu-id="dfc1b-117">String</span></span>|<span data-ttu-id="dfc1b-p102">既定のメッセージを送信する言語。customizedMessageBody が指定されている場合、このプロパティは無視され、メッセージは ustomizedMessageBody を使用して送信されます。言語書式は ISO 639 である必要があります。既定では ja-JP です。</span><span class="sxs-lookup"><span data-stu-id="dfc1b-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfc1b-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfc1b-122">JSON representation</span></span>
<span data-ttu-id="dfc1b-123">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="dfc1b-123">Here is a JSON representation of the resource</span></span>

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
