---
title: automaticRepliesSetting リソースの種類
description: '受信メールの送信者にメッセージを自動的に通知するための構成設定 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3a4320a687ca47d89e04d61c659075cea7722e32
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013158"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="7e17d-103">automaticRepliesSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e17d-103">automaticRepliesSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e17d-p101">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。たとえば、サインイン ユーザーが電子メールに返信できないことを通知する自動返信などです。</span><span class="sxs-lookup"><span data-stu-id="7e17d-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="7e17d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e17d-106">Properties</span></span>
| <span data-ttu-id="7e17d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e17d-107">Property</span></span>     | <span data-ttu-id="7e17d-108">型</span><span class="sxs-lookup"><span data-stu-id="7e17d-108">Type</span></span>   |<span data-ttu-id="7e17d-109">説明</span><span class="sxs-lookup"><span data-stu-id="7e17d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e17d-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="7e17d-110">externalAudience</span></span>|<span data-ttu-id="7e17d-111">String</span><span class="sxs-lookup"><span data-stu-id="7e17d-111">String</span></span>| <span data-ttu-id="7e17d-p102">**Status** が \*\*\*\* または `AlwaysEnabled` の場合に、`Scheduled` を受信する、サインイン ユーザーの組織外の一連の対象ユーザー。可能な値は、`none`、`contactsOnly`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="7e17d-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="7e17d-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="7e17d-114">externalReplyMessage</span></span>|<span data-ttu-id="7e17d-115">string</span><span class="sxs-lookup"><span data-stu-id="7e17d-115">string</span></span>|<span data-ttu-id="7e17d-116">**Status** が `AlwaysEnabled` または `Scheduled` の場合、指定の外部対象ユーザーに送信される自動応答。</span><span class="sxs-lookup"><span data-stu-id="7e17d-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="7e17d-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="7e17d-117">internalReplyMessage</span></span>|<span data-ttu-id="7e17d-118">string</span><span class="sxs-lookup"><span data-stu-id="7e17d-118">string</span></span>|<span data-ttu-id="7e17d-119">**Status** が `AlwaysEnabled` または `Scheduled` の場合、サインイン ユーザーの組織内の対象ユーザーに送信される自動応答。</span><span class="sxs-lookup"><span data-stu-id="7e17d-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="7e17d-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="7e17d-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="7e17d-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7e17d-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="7e17d-122">**Status** が `Scheduled` に設定されている場合に、自動応答を終了する日時。</span><span class="sxs-lookup"><span data-stu-id="7e17d-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="7e17d-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="7e17d-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="7e17d-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7e17d-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="7e17d-125">**Status** が `Scheduled` に設定されている場合に、自動応答を開始する日時。</span><span class="sxs-lookup"><span data-stu-id="7e17d-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="7e17d-126">status</span><span class="sxs-lookup"><span data-stu-id="7e17d-126">status</span></span>|<span data-ttu-id="7e17d-127">String</span><span class="sxs-lookup"><span data-stu-id="7e17d-127">String</span></span>|<span data-ttu-id="7e17d-p103">自動応答の構成状態。可能な値は、`disabled`、`alwaysEnabled`、`scheduled` です。</span><span class="sxs-lookup"><span data-stu-id="7e17d-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e17d-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e17d-130">JSON representation</span></span>

<span data-ttu-id="7e17d-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e17d-131">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
