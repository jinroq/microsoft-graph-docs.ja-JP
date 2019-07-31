---
title: 招待メッセージの構成
description: InvitedUserMessageInfo オブジェクトを使用すると、招待メッセージを構成できます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1c9fffd2edec48fb528dcb2f6c5a751dd4f32d30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010106"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="f32d0-103">招待メッセージの構成</span><span class="sxs-lookup"><span data-stu-id="f32d0-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f32d0-104">InvitedUserMessageInfo オブジェクトを使用すると、[招待](invitation.md)メッセージを構成できます。</span><span class="sxs-lookup"><span data-stu-id="f32d0-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="f32d0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f32d0-105">Properties</span></span>
| <span data-ttu-id="f32d0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f32d0-106">Property</span></span>     | <span data-ttu-id="f32d0-107">型</span><span class="sxs-lookup"><span data-stu-id="f32d0-107">Type</span></span>   |<span data-ttu-id="f32d0-108">説明</span><span class="sxs-lookup"><span data-stu-id="f32d0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f32d0-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="f32d0-109">ccRecipients</span></span>|<span data-ttu-id="f32d0-110">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="f32d0-110">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="f32d0-111">その他の受信者に招待メッセージを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f32d0-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="f32d0-112">現時点では、1つの追加の受信者のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f32d0-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="f32d0-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="f32d0-113">customizedMessageBody</span></span>|<span data-ttu-id="f32d0-114">String</span><span class="sxs-lookup"><span data-stu-id="f32d0-114">String</span></span>|<span data-ttu-id="f32d0-115">既定のメッセージを必要としない場合に送信する、カスタマイズされたメッセージ本文。</span><span class="sxs-lookup"><span data-stu-id="f32d0-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="f32d0-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="f32d0-116">messageLanguage</span></span>|<span data-ttu-id="f32d0-117">String</span><span class="sxs-lookup"><span data-stu-id="f32d0-117">String</span></span>|<span data-ttu-id="f32d0-118">既定のメッセージを送信する言語を指定します。</span><span class="sxs-lookup"><span data-stu-id="f32d0-118">The language you want to send the default message in.</span></span> <span data-ttu-id="f32d0-119">CustomizedMessageBody が指定されている場合、このプロパティは無視され、customizedMessageBody を使用してメッセージが送信されます。</span><span class="sxs-lookup"><span data-stu-id="f32d0-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="f32d0-120">言語の形式は ISO 639 である必要があります。</span><span class="sxs-lookup"><span data-stu-id="f32d0-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="f32d0-121">既定値は en-us です。</span><span class="sxs-lookup"><span data-stu-id="f32d0-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f32d0-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f32d0-122">JSON representation</span></span>
<span data-ttu-id="f32d0-123">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f32d0-123">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
