---
title: followupFlag リソースの種類
description: ユーザーが特定のアイテムを後でフォローアップできるよう、フラグを設定できます。 サポートされているアイテムには、メッセージと連絡先があります。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28f60187fcfb3d41779547b6252edf69c1fc2735
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971978"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="8808b-104">followupFlag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8808b-104">followupFlag resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8808b-105">ユーザーが特定のアイテムを後でフォローアップできるよう、フラグを設定できます。</span><span class="sxs-lookup"><span data-stu-id="8808b-105">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="8808b-106">サポートされているアイテムには、[メッセージ](message.md)と[連絡先](contact.md)があります。</span><span class="sxs-lookup"><span data-stu-id="8808b-106">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8808b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8808b-107">Properties</span></span>
| <span data-ttu-id="8808b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8808b-108">Property</span></span>     | <span data-ttu-id="8808b-109">型</span><span class="sxs-lookup"><span data-stu-id="8808b-109">Type</span></span>   |<span data-ttu-id="8808b-110">説明</span><span class="sxs-lookup"><span data-stu-id="8808b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8808b-111">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="8808b-111">completedDateTime</span></span>|[<span data-ttu-id="8808b-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8808b-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="8808b-113">フォローアップが終了した日時。</span><span class="sxs-lookup"><span data-stu-id="8808b-113">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="8808b-114">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="8808b-114">dueDateTime</span></span>|<span data-ttu-id="8808b-115">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="8808b-115">**dateTimeTimeZone**</span></span>|<span data-ttu-id="8808b-116">フォローアップが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="8808b-116">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="8808b-117">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="8808b-117">flagStatus</span></span>|<span data-ttu-id="8808b-118">String</span><span class="sxs-lookup"><span data-stu-id="8808b-118">String</span></span>|<span data-ttu-id="8808b-119">アイテムのフォローアップ状態。</span><span class="sxs-lookup"><span data-stu-id="8808b-119">The status for follow-up for an item.</span></span> <span data-ttu-id="8808b-120">可能な値は、`notFlagged`、`complete`、`flagged` です。</span><span class="sxs-lookup"><span data-stu-id="8808b-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="8808b-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8808b-121">startDateTime</span></span>|<span data-ttu-id="8808b-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="8808b-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="8808b-123">フォローアップを開始する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="8808b-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8808b-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8808b-124">JSON representation</span></span>

<span data-ttu-id="8808b-125">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8808b-125">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
