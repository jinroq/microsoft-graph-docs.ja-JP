---
title: 招待メッセージの構成
description: invitedUserMessageInfo オブジェクトでは、招待メッセージを構成できます。
localization_priority: Normal
ms.openlocfilehash: 06be157e61fd6d466cc2b18546bb29762d0133a8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885870"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="8bb84-103">招待メッセージの構成</span><span class="sxs-lookup"><span data-stu-id="8bb84-103">Configuring the invitation message</span></span>

<span data-ttu-id="8bb84-104">invitedUserMessageInfo オブジェクトでは、[招待](invitation.md)メッセージを構成できます。</span><span class="sxs-lookup"><span data-stu-id="8bb84-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="8bb84-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bb84-105">Properties</span></span>
| <span data-ttu-id="8bb84-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bb84-106">Property</span></span>     | <span data-ttu-id="8bb84-107">種類</span><span class="sxs-lookup"><span data-stu-id="8bb84-107">Type</span></span>   |<span data-ttu-id="8bb84-108">説明</span><span class="sxs-lookup"><span data-stu-id="8bb84-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bb84-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="8bb84-109">ccRecipients</span></span>|<span data-ttu-id="8bb84-110">[Recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="8bb84-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="8bb84-p101">招待メッセージの送信先にする必要がある追加の受信者。現在、サポートされている追加の受信者は 1 人のみです。</span><span class="sxs-lookup"><span data-stu-id="8bb84-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="8bb84-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="8bb84-113">customizedMessageBody</span></span>|<span data-ttu-id="8bb84-114">String</span><span class="sxs-lookup"><span data-stu-id="8bb84-114">String</span></span>|<span data-ttu-id="8bb84-115">既定のメッセージを使用しない場合に送信するカスタマイズされたメッセージ本文。</span><span class="sxs-lookup"><span data-stu-id="8bb84-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="8bb84-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="8bb84-116">messageLanguage</span></span>|<span data-ttu-id="8bb84-117">String</span><span class="sxs-lookup"><span data-stu-id="8bb84-117">String</span></span>|<span data-ttu-id="8bb84-p102">既定のメッセージを送信する言語。customizedMessageBody が指定されている場合、このプロパティは無視され、メッセージは ustomizedMessageBody を使用して送信されます。言語書式は ISO 639 である必要があります。既定では ja-JP です。</span><span class="sxs-lookup"><span data-stu-id="8bb84-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bb84-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8bb84-122">JSON representation</span></span>
<span data-ttu-id="8bb84-123">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8bb84-123">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
