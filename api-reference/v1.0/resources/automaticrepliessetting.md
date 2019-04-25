---
title: automaticRepliesSetting リソースの種類
description: '受信メールの送信者にメッセージを自動的に通知するための構成設定 '
localization_priority: Normal
ms.openlocfilehash: 81fb16a9124c60f43887150917f132579aa4f163
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569425"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="069e1-103">automaticRepliesSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="069e1-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="069e1-p101">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。たとえば、サインイン ユーザーが電子メールに返信できないことを通知する自動返信などです。</span><span class="sxs-lookup"><span data-stu-id="069e1-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="069e1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="069e1-106">Properties</span></span>
| <span data-ttu-id="069e1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="069e1-107">Property</span></span>     | <span data-ttu-id="069e1-108">型</span><span class="sxs-lookup"><span data-stu-id="069e1-108">Type</span></span>   |<span data-ttu-id="069e1-109">説明</span><span class="sxs-lookup"><span data-stu-id="069e1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="069e1-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="069e1-110">externalAudience</span></span>|<span data-ttu-id="069e1-111">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="069e1-111">externalAudienceScope</span></span>| <span data-ttu-id="069e1-112">**Status** が \*\*\*\* または `AlwaysEnabled` の場合に、`Scheduled` を受信する、サインイン ユーザーの組織外の一連の対象ユーザー。</span><span class="sxs-lookup"><span data-stu-id="069e1-112">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="069e1-113">使用可能な値: `none`、`contactsOnly`、`all`。</span><span class="sxs-lookup"><span data-stu-id="069e1-113">The possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="069e1-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="069e1-114">externalReplyMessage</span></span>|<span data-ttu-id="069e1-115">string</span><span class="sxs-lookup"><span data-stu-id="069e1-115">string</span></span>|<span data-ttu-id="069e1-116">**Status** が `AlwaysEnabled` または `Scheduled` の場合、指定の外部対象ユーザーに送信される自動応答。</span><span class="sxs-lookup"><span data-stu-id="069e1-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="069e1-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="069e1-117">internalReplyMessage</span></span>|<span data-ttu-id="069e1-118">string</span><span class="sxs-lookup"><span data-stu-id="069e1-118">string</span></span>|<span data-ttu-id="069e1-119">**Status** が `AlwaysEnabled` または `Scheduled` の場合、サインイン ユーザーの組織内の対象ユーザーに送信される自動応答。</span><span class="sxs-lookup"><span data-stu-id="069e1-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="069e1-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="069e1-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="069e1-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="069e1-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="069e1-122">**Status** が `Scheduled` に設定されている場合に、自動応答を終了する日時。</span><span class="sxs-lookup"><span data-stu-id="069e1-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="069e1-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="069e1-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="069e1-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="069e1-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="069e1-125">**Status** が `Scheduled` に設定されている場合に、自動応答を開始する日時。</span><span class="sxs-lookup"><span data-stu-id="069e1-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="069e1-126">status</span><span class="sxs-lookup"><span data-stu-id="069e1-126">status</span></span>|<span data-ttu-id="069e1-127">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="069e1-127">automaticRepliesStatus</span></span>|<span data-ttu-id="069e1-128">自動応答の構成状態。</span><span class="sxs-lookup"><span data-stu-id="069e1-128">Configurations status for automatic replies.</span></span> <span data-ttu-id="069e1-129">使用可能な値: `disabled`、`alwaysEnabled`、`scheduled`。</span><span class="sxs-lookup"><span data-stu-id="069e1-129">The possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="069e1-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="069e1-130">JSON representation</span></span>

<span data-ttu-id="069e1-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="069e1-131">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
