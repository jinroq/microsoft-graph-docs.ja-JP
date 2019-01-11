---
title: 招待メッセージの構成
description: invitedUserMessageInfo オブジェクトでは、招待メッセージを構成できます。
localization_priority: Normal
ms.openlocfilehash: f8a6dd118f1774320e3fe8327d284dac1141fc55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874124"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="86002-103">招待メッセージの構成</span><span class="sxs-lookup"><span data-stu-id="86002-103">Configuring the invitation message</span></span>

> <span data-ttu-id="86002-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86002-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86002-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86002-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86002-106">invitedUserMessageInfo オブジェクトでは、[招待](invitation.md)メッセージを構成できます。</span><span class="sxs-lookup"><span data-stu-id="86002-106">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="86002-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86002-107">Properties</span></span>
| <span data-ttu-id="86002-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86002-108">Property</span></span>     | <span data-ttu-id="86002-109">種類</span><span class="sxs-lookup"><span data-stu-id="86002-109">Type</span></span>   |<span data-ttu-id="86002-110">説明</span><span class="sxs-lookup"><span data-stu-id="86002-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86002-111">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="86002-111">ccRecipients</span></span>|[<span data-ttu-id="86002-112">受信者</span><span class="sxs-lookup"><span data-stu-id="86002-112">Recipients</span></span>](recipient.md)|<span data-ttu-id="86002-p102">招待メッセージの送信先にする必要がある追加の受信者。現在、サポートされている追加の受信者は 1 人のみです。</span><span class="sxs-lookup"><span data-stu-id="86002-p102">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="86002-115">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="86002-115">customizedMessageBody</span></span>|<span data-ttu-id="86002-116">String</span><span class="sxs-lookup"><span data-stu-id="86002-116">String</span></span>|<span data-ttu-id="86002-117">既定のメッセージを使用しない場合に送信するカスタマイズされたメッセージ本文。</span><span class="sxs-lookup"><span data-stu-id="86002-117">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="86002-118">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="86002-118">messageLanguage</span></span>|<span data-ttu-id="86002-119">String</span><span class="sxs-lookup"><span data-stu-id="86002-119">String</span></span>|<span data-ttu-id="86002-p103">既定のメッセージを送信する言語。customizedMessageBody が指定されている場合、このプロパティは無視され、メッセージは ustomizedMessageBody を使用して送信されます。言語書式は ISO 639 である必要があります。既定では ja-JP です。</span><span class="sxs-lookup"><span data-stu-id="86002-p103">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86002-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86002-124">JSON representation</span></span>
<span data-ttu-id="86002-125">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="86002-125">Here is a JSON representation of the resource</span></span>

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
