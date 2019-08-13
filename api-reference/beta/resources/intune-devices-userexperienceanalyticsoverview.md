---
title: userExperienceAnalyticsOverview リソースの種類
description: User experience analytics の概要エンティティには、全体的なスコアと、すべてのカテゴリのすべてのメトリックのスコアと洞察が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff3be73059f913943236bfce8bcb4e729a39081d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371524"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="bb0e4-103">userExperienceAnalyticsOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb0e4-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="bb0e4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb0e4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb0e4-106">User experience analytics の概要エンティティには、全体的なスコアと、すべてのカテゴリのすべてのメトリックのスコアと洞察が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="bb0e4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb0e4-107">Methods</span></span>
|<span data-ttu-id="bb0e4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb0e4-108">Method</span></span>|<span data-ttu-id="bb0e4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb0e4-109">Return Type</span></span>|<span data-ttu-id="bb0e4-110">説明</span><span class="sxs-lookup"><span data-stu-id="bb0e4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb0e4-111">UserExperienceAnalyticsOverview を取得する</span><span class="sxs-lookup"><span data-stu-id="bb0e4-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="bb0e4-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="bb0e4-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="bb0e4-113">[UserExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="bb0e4-114">UserExperienceAnalyticsOverview の更新</span><span class="sxs-lookup"><span data-stu-id="bb0e4-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="bb0e4-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="bb0e4-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="bb0e4-116">[UserExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb0e4-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb0e4-117">Properties</span></span>
|<span data-ttu-id="bb0e4-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb0e4-118">Property</span></span>|<span data-ttu-id="bb0e4-119">型</span><span class="sxs-lookup"><span data-stu-id="bb0e4-119">Type</span></span>|<span data-ttu-id="bb0e4-120">説明</span><span class="sxs-lookup"><span data-stu-id="bb0e4-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb0e4-121">id</span><span class="sxs-lookup"><span data-stu-id="bb0e4-121">id</span></span>|<span data-ttu-id="bb0e4-122">String</span><span class="sxs-lookup"><span data-stu-id="bb0e4-122">String</span></span>|<span data-ttu-id="bb0e4-123">ユーザー experience analytics の概要の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="bb0e4-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="bb0e4-124">overallScore</span></span>|<span data-ttu-id="bb0e4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0e4-125">Int32</span></span>|<span data-ttu-id="bb0e4-126">ユーザー experience analytics 総合得点。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="bb0e4-127">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="bb0e4-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="bb0e4-128">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0e4-128">Int32</span></span>|<span data-ttu-id="bb0e4-129">ユーザーが analytics デバイスのブートパフォーマンス全体スコアを表示します。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="bb0e4-130">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="bb0e4-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="bb0e4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0e4-131">Int32</span></span>|<span data-ttu-id="bb0e4-132">ユーザー操作分析のベストプラクティス全体のスコア。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="bb0e4-133">insights</span><span class="sxs-lookup"><span data-stu-id="bb0e4-133">insights</span></span>|<span data-ttu-id="bb0e4-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb0e4-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="bb0e4-135">ユーザー experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-135">The user experience analytics insights.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb0e4-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb0e4-136">Relationships</span></span>
<span data-ttu-id="bb0e4-137">なし</span><span class="sxs-lookup"><span data-stu-id="bb0e4-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb0e4-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb0e4-138">JSON Representation</span></span>
<span data-ttu-id="bb0e4-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb0e4-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": 1024,
  "deviceBootPerformanceOverallScore": 1024,
  "bestPracticesOverallScore": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```



