---
title: accessReviewSettings リソースの種類
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348406"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="ff674-102">accessReviewSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff674-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="ff674-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff674-103">Properties</span></span>
|<span data-ttu-id="ff674-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff674-104">Property</span></span>|<span data-ttu-id="ff674-105">型</span><span class="sxs-lookup"><span data-stu-id="ff674-105">Type</span></span>|<span data-ttu-id="ff674-106">説明</span><span class="sxs-lookup"><span data-stu-id="ff674-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="ff674-107">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="ff674-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="ff674-108">boolean</span><span class="sxs-lookup"><span data-stu-id="ff674-108">boolean</span></span> |  |
| <span data-ttu-id="ff674-109">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="ff674-109">remindersEnabled</span></span> | <span data-ttu-id="ff674-110">boolean</span><span class="sxs-lookup"><span data-stu-id="ff674-110">boolean</span></span> |  |
| <span data-ttu-id="ff674-111">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="ff674-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="ff674-112">boolean</span><span class="sxs-lookup"><span data-stu-id="ff674-112">boolean</span></span> |  |
| <span data-ttu-id="ff674-113">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="ff674-113">recurrenceSettings</span></span> | <span data-ttu-id="ff674-114">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="ff674-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="ff674-115">autoreviewenabled</span><span class="sxs-lookup"><span data-stu-id="ff674-115">autoReviewEnabled</span></span> | <span data-ttu-id="ff674-116">boolean</span><span class="sxs-lookup"><span data-stu-id="ff674-116">boolean</span></span> |  |
| <span data-ttu-id="ff674-117">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="ff674-117">activityDurationInDays</span></span> | <span data-ttu-id="ff674-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ff674-118">Int32</span></span> |  |
| <span data-ttu-id="ff674-119">autoreviewsettings</span><span class="sxs-lookup"><span data-stu-id="ff674-119">autoReviewSettings</span></span> | <span data-ttu-id="ff674-120">autoreviewsettings</span><span class="sxs-lookup"><span data-stu-id="ff674-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="ff674-121">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="ff674-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="ff674-122">boolean</span><span class="sxs-lookup"><span data-stu-id="ff674-122">boolean</span></span> |  |
| <span data-ttu-id="ff674-123">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="ff674-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="ff674-124">boolean</span><span class="sxs-lookup"><span data-stu-id="ff674-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="ff674-125">関係</span><span class="sxs-lookup"><span data-stu-id="ff674-125">Relationships</span></span>
<span data-ttu-id="ff674-126">なし</span><span class="sxs-lookup"><span data-stu-id="ff674-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff674-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff674-127">JSON Representation</span></span>
<span data-ttu-id="ff674-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff674-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
``` json
{
    "mailNotificationsEnabled":"boolean",
    "remindersEnabled":"boolean",
    "justificationRequiredOnApproval":"boolean",
    "recurrenceSettings":"microsoft.graph.accessReviewRecurrenceSettings",
    "autoReviewEnabled":"boolean",
    "activityDurationInDays":"Int32",
    "autoReviewSettings":"microsoft.graph.autoReviewSettings",
    "autoApplyReviewResultsEnabled":"boolean",
    "accessRecommendationsEnabled":"boolean"
}
```



