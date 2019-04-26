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
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="9afed-103">招待メッセージの構成</span><span class="sxs-lookup"><span data-stu-id="9afed-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9afed-104">invitedUserMessageInfo オブジェクトを使用すると、[招待](invitation.md)メッセージを構成できます。</span><span class="sxs-lookup"><span data-stu-id="9afed-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="9afed-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9afed-105">Properties</span></span>
| <span data-ttu-id="9afed-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9afed-106">Property</span></span>     | <span data-ttu-id="9afed-107">型</span><span class="sxs-lookup"><span data-stu-id="9afed-107">Type</span></span>   |<span data-ttu-id="9afed-108">説明</span><span class="sxs-lookup"><span data-stu-id="9afed-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9afed-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="9afed-109">ccRecipients</span></span>|[<span data-ttu-id="9afed-110">受信者</span><span class="sxs-lookup"><span data-stu-id="9afed-110">Recipients</span></span>](recipient.md)|<span data-ttu-id="9afed-111">その他の受信者に招待メッセージを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9afed-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="9afed-112">現時点では、1つの追加の受信者のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9afed-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="9afed-113">customizedmessagebody</span><span class="sxs-lookup"><span data-stu-id="9afed-113">customizedMessageBody</span></span>|<span data-ttu-id="9afed-114">String</span><span class="sxs-lookup"><span data-stu-id="9afed-114">String</span></span>|<span data-ttu-id="9afed-115">既定のメッセージを必要としない場合に送信する、カスタマイズされたメッセージ本文。</span><span class="sxs-lookup"><span data-stu-id="9afed-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="9afed-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="9afed-116">messageLanguage</span></span>|<span data-ttu-id="9afed-117">String</span><span class="sxs-lookup"><span data-stu-id="9afed-117">String</span></span>|<span data-ttu-id="9afed-118">既定のメッセージを送信する言語を指定します。</span><span class="sxs-lookup"><span data-stu-id="9afed-118">The language you want to send the default message in.</span></span> <span data-ttu-id="9afed-119">customizedmessagebody が指定されている場合、このプロパティは無視され、customizedmessagebody を使用してメッセージが送信されます。</span><span class="sxs-lookup"><span data-stu-id="9afed-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="9afed-120">言語の形式は ISO 639 である必要があります。</span><span class="sxs-lookup"><span data-stu-id="9afed-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="9afed-121">既定値は en-us です。</span><span class="sxs-lookup"><span data-stu-id="9afed-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9afed-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9afed-122">JSON representation</span></span>
<span data-ttu-id="9afed-123">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9afed-123">Here is a JSON representation of the resource</span></span>

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
