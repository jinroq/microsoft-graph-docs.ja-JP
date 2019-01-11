---
title: followupFlag リソースの種類
description: ユーザーが特定のアイテムを後でフォローアップできるよう、フラグを設定できます。 サポートされているアイテムには、メッセージと連絡先があります。
localization_priority: Normal
ms.openlocfilehash: aa056d141bfac82b9f039ed705f6de49893783fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869379"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="468c7-104">followupFlag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="468c7-104">followupFlag resource type</span></span>

> <span data-ttu-id="468c7-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="468c7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="468c7-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="468c7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="468c7-107">ユーザーが特定のアイテムを後でフォローアップできるよう、フラグを設定できます。</span><span class="sxs-lookup"><span data-stu-id="468c7-107">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="468c7-108">サポートされているアイテムには、[メッセージ](message.md)と[連絡先](contact.md)があります。</span><span class="sxs-lookup"><span data-stu-id="468c7-108">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="468c7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="468c7-109">Properties</span></span>
| <span data-ttu-id="468c7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="468c7-110">Property</span></span>     | <span data-ttu-id="468c7-111">種類</span><span class="sxs-lookup"><span data-stu-id="468c7-111">Type</span></span>   |<span data-ttu-id="468c7-112">説明</span><span class="sxs-lookup"><span data-stu-id="468c7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="468c7-113">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="468c7-113">completedDateTime</span></span>|[<span data-ttu-id="468c7-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="468c7-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="468c7-115">フォローアップが終了した日時。</span><span class="sxs-lookup"><span data-stu-id="468c7-115">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="468c7-116">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="468c7-116">dueDateTime</span></span>|<span data-ttu-id="468c7-117">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="468c7-117">**dateTimeTimeZone**</span></span>|<span data-ttu-id="468c7-118">フォローアップが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="468c7-118">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="468c7-119">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="468c7-119">flagStatus</span></span>|<span data-ttu-id="468c7-120">String</span><span class="sxs-lookup"><span data-stu-id="468c7-120">String</span></span>|<span data-ttu-id="468c7-121">アイテムのフォローアップ状態。</span><span class="sxs-lookup"><span data-stu-id="468c7-121">The status for follow-up for an item.</span></span> <span data-ttu-id="468c7-122">可能な値は、`notFlagged`、`complete`、`flagged` です。</span><span class="sxs-lookup"><span data-stu-id="468c7-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="468c7-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="468c7-123">startDateTime</span></span>|<span data-ttu-id="468c7-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="468c7-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="468c7-125">フォローアップを開始する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="468c7-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="468c7-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="468c7-126">JSON representation</span></span>

<span data-ttu-id="468c7-127">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="468c7-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
