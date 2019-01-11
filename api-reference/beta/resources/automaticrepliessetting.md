---
title: automaticRepliesSetting リソースの種類
description: 'メッセージを受信したメールの送信者に自動的に通知する設定を構成します '
localization_priority: Normal
ms.openlocfilehash: 0160197a4fafe10b7f78be9124da3b6260bfcee6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820658"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="a7fee-103">automaticRepliesSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7fee-103">automaticRepliesSetting resource type</span></span>

> <span data-ttu-id="a7fee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a7fee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7fee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7fee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7fee-p102">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。たとえば、サインイン ユーザーが電子メールに返信できないことを通知する自動返信などです。</span><span class="sxs-lookup"><span data-stu-id="a7fee-p102">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="a7fee-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7fee-108">Properties</span></span>
| <span data-ttu-id="a7fee-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7fee-109">Property</span></span>     | <span data-ttu-id="a7fee-110">種類</span><span class="sxs-lookup"><span data-stu-id="a7fee-110">Type</span></span>   |<span data-ttu-id="a7fee-111">説明</span><span class="sxs-lookup"><span data-stu-id="a7fee-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7fee-112">externalAudience</span><span class="sxs-lookup"><span data-stu-id="a7fee-112">externalAudience</span></span>|<span data-ttu-id="a7fee-113">String</span><span class="sxs-lookup"><span data-stu-id="a7fee-113">String</span></span>| <span data-ttu-id="a7fee-p103">**Status** が `AlwaysEnabled` または `Scheduled` の場合に、**ExternalReplyMessage** を受信する、サインイン ユーザーの組織外の一連の対象ユーザー。可能な値は、`none`、`contactsOnly`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="a7fee-p103">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="a7fee-116">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="a7fee-116">externalReplyMessage</span></span>|<span data-ttu-id="a7fee-117">文字列</span><span class="sxs-lookup"><span data-stu-id="a7fee-117">string</span></span>|<span data-ttu-id="a7fee-118">**Status** が `AlwaysEnabled` または `Scheduled` の場合、指定の外部対象ユーザーに送信される自動応答。</span><span class="sxs-lookup"><span data-stu-id="a7fee-118">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="a7fee-119">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="a7fee-119">internalReplyMessage</span></span>|<span data-ttu-id="a7fee-120">文字列</span><span class="sxs-lookup"><span data-stu-id="a7fee-120">string</span></span>|<span data-ttu-id="a7fee-121">**Status** が `AlwaysEnabled` または `Scheduled` の場合、サインイン ユーザーの組織内の対象ユーザーに送信される自動応答。</span><span class="sxs-lookup"><span data-stu-id="a7fee-121">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="a7fee-122">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="a7fee-122">scheduledEndDateTime</span></span>|[<span data-ttu-id="a7fee-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a7fee-123">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a7fee-124">**Status** が `Scheduled` に設定されている場合に、自動応答を終了する日時。</span><span class="sxs-lookup"><span data-stu-id="a7fee-124">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="a7fee-125">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a7fee-125">scheduledStartDateTime</span></span>|[<span data-ttu-id="a7fee-126">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a7fee-126">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a7fee-127">**Status** が `Scheduled` に設定されている場合に、自動応答を開始する日時。</span><span class="sxs-lookup"><span data-stu-id="a7fee-127">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="a7fee-128">status</span><span class="sxs-lookup"><span data-stu-id="a7fee-128">status</span></span>|<span data-ttu-id="a7fee-129">String</span><span class="sxs-lookup"><span data-stu-id="a7fee-129">String</span></span>|<span data-ttu-id="a7fee-p104">自動応答の構成状態。可能な値は、`disabled`、`alwaysEnabled`、`scheduled` です。</span><span class="sxs-lookup"><span data-stu-id="a7fee-p104">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7fee-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7fee-132">JSON representation</span></span>

<span data-ttu-id="a7fee-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7fee-133">Here is a JSON representation of the resource.</span></span>

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
