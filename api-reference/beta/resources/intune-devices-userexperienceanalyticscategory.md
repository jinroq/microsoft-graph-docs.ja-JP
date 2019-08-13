---
title: userExperienceAnalyticsCategory リソースの種類
description: User experience analytics category エンティティには、カテゴリのさまざまな指標のスコアと洞察が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c04f2caaa7b9ee6c093a58e4c8123250113b3a9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329647"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="a065c-103">userExperienceAnalyticsCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a065c-103">userExperienceAnalyticsCategory resource type</span></span>

> <span data-ttu-id="a065c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a065c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a065c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a065c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a065c-106">User experience analytics category エンティティには、カテゴリのさまざまな指標のスコアと洞察が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a065c-106">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="a065c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a065c-107">Methods</span></span>
|<span data-ttu-id="a065c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a065c-108">Method</span></span>|<span data-ttu-id="a065c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a065c-109">Return Type</span></span>|<span data-ttu-id="a065c-110">説明</span><span class="sxs-lookup"><span data-stu-id="a065c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a065c-111">UserExperienceAnalyticsCategory を取得する</span><span class="sxs-lookup"><span data-stu-id="a065c-111">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="a065c-112">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="a065c-112">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="a065c-113">[UserExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a065c-113">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="a065c-114">UserExperienceAnalyticsCategory の更新</span><span class="sxs-lookup"><span data-stu-id="a065c-114">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="a065c-115">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="a065c-115">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="a065c-116">[UserExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a065c-116">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a065c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a065c-117">Properties</span></span>
|<span data-ttu-id="a065c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a065c-118">Property</span></span>|<span data-ttu-id="a065c-119">型</span><span class="sxs-lookup"><span data-stu-id="a065c-119">Type</span></span>|<span data-ttu-id="a065c-120">説明</span><span class="sxs-lookup"><span data-stu-id="a065c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a065c-121">id</span><span class="sxs-lookup"><span data-stu-id="a065c-121">id</span></span>|<span data-ttu-id="a065c-122">文字列</span><span class="sxs-lookup"><span data-stu-id="a065c-122">String</span></span>|<span data-ttu-id="a065c-123">ユーザー experience analytics カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a065c-123">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="a065c-124">displayName</span><span class="sxs-lookup"><span data-stu-id="a065c-124">displayName</span></span>|<span data-ttu-id="a065c-125">String</span><span class="sxs-lookup"><span data-stu-id="a065c-125">String</span></span>|<span data-ttu-id="a065c-126">ユーザー experience analytics カテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="a065c-126">The name of the user experience analytics category.</span></span>|
|<span data-ttu-id="a065c-127">overallScore</span><span class="sxs-lookup"><span data-stu-id="a065c-127">overallScore</span></span>|<span data-ttu-id="a065c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a065c-128">Int32</span></span>|<span data-ttu-id="a065c-129">ユーザー experience analytics カテゴリの全体的なスコア。</span><span class="sxs-lookup"><span data-stu-id="a065c-129">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="a065c-130">insights</span><span class="sxs-lookup"><span data-stu-id="a065c-130">insights</span></span>|<span data-ttu-id="a065c-131">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a065c-131">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="a065c-132">ユーザー experience analytics カテゴリの洞察。</span><span class="sxs-lookup"><span data-stu-id="a065c-132">The insights for the user experience analytics category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a065c-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a065c-133">Relationships</span></span>
|<span data-ttu-id="a065c-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a065c-134">Relationship</span></span>|<span data-ttu-id="a065c-135">型</span><span class="sxs-lookup"><span data-stu-id="a065c-135">Type</span></span>|<span data-ttu-id="a065c-136">説明</span><span class="sxs-lookup"><span data-stu-id="a065c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a065c-137">metricValues</span><span class="sxs-lookup"><span data-stu-id="a065c-137">metricValues</span></span>|<span data-ttu-id="a065c-138">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a065c-138">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="a065c-139">ユーザー experience analytics カテゴリのメトリック値。</span><span class="sxs-lookup"><span data-stu-id="a065c-139">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a065c-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a065c-140">JSON Representation</span></span>
<span data-ttu-id="a065c-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a065c-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
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



