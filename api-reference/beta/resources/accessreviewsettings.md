---
title: accessReviewSettings リソースの種類
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 2c51d94b3143d9929c03093cfb1a6625d6a9e3db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974538"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="7557b-102">accessReviewSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7557b-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="7557b-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7557b-103">Properties</span></span>
|<span data-ttu-id="7557b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7557b-104">Property</span></span>|<span data-ttu-id="7557b-105">型</span><span class="sxs-lookup"><span data-stu-id="7557b-105">Type</span></span>|<span data-ttu-id="7557b-106">説明</span><span class="sxs-lookup"><span data-stu-id="7557b-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="7557b-107">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="7557b-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="7557b-108">ブール値</span><span class="sxs-lookup"><span data-stu-id="7557b-108">boolean</span></span> |  |
| <span data-ttu-id="7557b-109">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="7557b-109">remindersEnabled</span></span> | <span data-ttu-id="7557b-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="7557b-110">boolean</span></span> |  |
| <span data-ttu-id="7557b-111">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="7557b-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="7557b-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="7557b-112">boolean</span></span> |  |
| <span data-ttu-id="7557b-113">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="7557b-113">recurrenceSettings</span></span> | <span data-ttu-id="7557b-114">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="7557b-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="7557b-115">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="7557b-115">autoReviewEnabled</span></span> | <span data-ttu-id="7557b-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="7557b-116">boolean</span></span> |  |
| <span data-ttu-id="7557b-117">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="7557b-117">activityDurationInDays</span></span> | <span data-ttu-id="7557b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="7557b-118">Int32</span></span> |  |
| <span data-ttu-id="7557b-119">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="7557b-119">autoReviewSettings</span></span> | <span data-ttu-id="7557b-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="7557b-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="7557b-121">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="7557b-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="7557b-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="7557b-122">boolean</span></span> |  |
| <span data-ttu-id="7557b-123">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="7557b-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="7557b-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="7557b-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="7557b-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7557b-125">Relationships</span></span>
<span data-ttu-id="7557b-126">なし</span><span class="sxs-lookup"><span data-stu-id="7557b-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7557b-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7557b-127">JSON Representation</span></span>
<span data-ttu-id="7557b-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7557b-128">Here is a JSON representation of the resource.</span></span>
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



