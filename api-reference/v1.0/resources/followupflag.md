---
title: followupFlag リソースの種類
description: 'ユーザーが後でフォローするためのアイテムにフラグを設定できます。 '
localization_priority: Normal
ms.openlocfilehash: 60d2e40a10c3ba5b2af9aa798b84aadaebedd57a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885499"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="81a67-103">followupFlag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81a67-103">followupFlag resource type</span></span>


<span data-ttu-id="81a67-104">ユーザーが後でフォローするためのアイテムにフラグを設定できます。</span><span class="sxs-lookup"><span data-stu-id="81a67-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="81a67-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81a67-105">Properties</span></span>
| <span data-ttu-id="81a67-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81a67-106">Property</span></span>     | <span data-ttu-id="81a67-107">種類</span><span class="sxs-lookup"><span data-stu-id="81a67-107">Type</span></span>   |<span data-ttu-id="81a67-108">説明</span><span class="sxs-lookup"><span data-stu-id="81a67-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a67-109">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="81a67-109">completedDateTime</span></span>|[<span data-ttu-id="81a67-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="81a67-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="81a67-111">フォローアップが終了した日時。</span><span class="sxs-lookup"><span data-stu-id="81a67-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="81a67-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="81a67-112">dueDateTime</span></span>|<span data-ttu-id="81a67-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="81a67-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="81a67-114">フォローアップが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="81a67-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="81a67-115">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="81a67-115">flagStatus</span></span>|<span data-ttu-id="81a67-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="81a67-116">followupFlagStatus</span></span>|<span data-ttu-id="81a67-117">アイテムのフォローアップ状態。</span><span class="sxs-lookup"><span data-stu-id="81a67-117">The status for follow-up for an item.</span></span> <span data-ttu-id="81a67-118">可能な値は、`notFlagged`、`complete`、`flagged` です。</span><span class="sxs-lookup"><span data-stu-id="81a67-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="81a67-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="81a67-119">startDateTime</span></span>|<span data-ttu-id="81a67-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="81a67-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="81a67-121">フォローアップを開始する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="81a67-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81a67-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81a67-122">JSON representation</span></span>

<span data-ttu-id="81a67-123">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="81a67-123">Here is a JSON representation of the resource</span></span>

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
