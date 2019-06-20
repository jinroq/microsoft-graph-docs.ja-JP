---
title: accessReviewSettings リソースの種類
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/20/2019
ms.locfileid: "35084069"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="d23d9-102">accessReviewSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d23d9-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="d23d9-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d23d9-103">Properties</span></span>
|<span data-ttu-id="d23d9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d23d9-104">Property</span></span>|<span data-ttu-id="d23d9-105">型</span><span class="sxs-lookup"><span data-stu-id="d23d9-105">Type</span></span>|<span data-ttu-id="d23d9-106">説明</span><span class="sxs-lookup"><span data-stu-id="d23d9-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="d23d9-107">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="d23d9-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="d23d9-108">ブール値</span><span class="sxs-lookup"><span data-stu-id="d23d9-108">boolean</span></span> |  |
| <span data-ttu-id="d23d9-109">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="d23d9-109">remindersEnabled</span></span> | <span data-ttu-id="d23d9-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="d23d9-110">boolean</span></span> |  |
| <span data-ttu-id="d23d9-111">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="d23d9-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="d23d9-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="d23d9-112">boolean</span></span> |  |
| <span data-ttu-id="d23d9-113">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="d23d9-113">recurrenceSettings</span></span> | <span data-ttu-id="d23d9-114">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="d23d9-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="d23d9-115">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="d23d9-115">autoReviewEnabled</span></span> | <span data-ttu-id="d23d9-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="d23d9-116">boolean</span></span> |  |
| <span data-ttu-id="d23d9-117">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="d23d9-117">activityDurationInDays</span></span> | <span data-ttu-id="d23d9-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d23d9-118">Int32</span></span> |  |
| <span data-ttu-id="d23d9-119">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="d23d9-119">autoReviewSettings</span></span> | <span data-ttu-id="d23d9-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="d23d9-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="d23d9-121">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="d23d9-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="d23d9-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="d23d9-122">boolean</span></span> |  |
| <span data-ttu-id="d23d9-123">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="d23d9-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="d23d9-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="d23d9-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="d23d9-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d23d9-125">Relationships</span></span>
<span data-ttu-id="d23d9-126">なし</span><span class="sxs-lookup"><span data-stu-id="d23d9-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d23d9-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d23d9-127">JSON Representation</span></span>
<span data-ttu-id="d23d9-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d23d9-128">Here is a JSON representation of the resource.</span></span>
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



