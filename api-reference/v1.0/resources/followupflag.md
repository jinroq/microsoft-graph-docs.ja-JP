---
title: followupFlag リソースの種類
description: 'ユーザーが後でフォローアップできるように、アイテムにフラグを設定することができます。 '
localization_priority: Normal
ms.openlocfilehash: 60d2e40a10c3ba5b2af9aa798b84aadaebedd57a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541998"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="fe2c6-103">followupFlag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe2c6-103">followupFlag resource type</span></span>


<span data-ttu-id="fe2c6-104">ユーザーが後でフォローアップできるように、アイテムにフラグを設定することができます。</span><span class="sxs-lookup"><span data-stu-id="fe2c6-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="fe2c6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe2c6-105">Properties</span></span>
| <span data-ttu-id="fe2c6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe2c6-106">Property</span></span>     | <span data-ttu-id="fe2c6-107">型</span><span class="sxs-lookup"><span data-stu-id="fe2c6-107">Type</span></span>   |<span data-ttu-id="fe2c6-108">説明</span><span class="sxs-lookup"><span data-stu-id="fe2c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe2c6-109">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe2c6-109">completedDateTime</span></span>|[<span data-ttu-id="fe2c6-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fe2c6-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="fe2c6-111">フォローアップが終了した日時。</span><span class="sxs-lookup"><span data-stu-id="fe2c6-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="fe2c6-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="fe2c6-112">dueDateTime</span></span>|<span data-ttu-id="fe2c6-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="fe2c6-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="fe2c6-114">フォローアップが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="fe2c6-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="fe2c6-115">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="fe2c6-115">flagStatus</span></span>|<span data-ttu-id="fe2c6-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="fe2c6-116">followupFlagStatus</span></span>|<span data-ttu-id="fe2c6-117">アイテムのフォローアップ状態。</span><span class="sxs-lookup"><span data-stu-id="fe2c6-117">The status for follow-up for an item.</span></span> <span data-ttu-id="fe2c6-118">可能な値は、`notFlagged`、`complete`、`flagged` です。</span><span class="sxs-lookup"><span data-stu-id="fe2c6-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="fe2c6-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fe2c6-119">startDateTime</span></span>|<span data-ttu-id="fe2c6-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="fe2c6-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="fe2c6-121">フォローアップを開始する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="fe2c6-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe2c6-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe2c6-122">JSON representation</span></span>

<span data-ttu-id="fe2c6-123">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fe2c6-123">Here is a JSON representation of the resource</span></span>

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
