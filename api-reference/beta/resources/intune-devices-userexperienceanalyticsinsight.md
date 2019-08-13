---
title: userExperienceAnalyticsInsight リソースの種類
description: ユーザーの分析に関する分析情報は、ユーザー環境分析のスコアを向上させるための推奨事項です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 36277b147e7eabc6f28aef3877538ebbc429f381
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341234"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="eb477-103">userExperienceAnalyticsInsight リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb477-103">userExperienceAnalyticsInsight resource type</span></span>

> <span data-ttu-id="eb477-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb477-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb477-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb477-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb477-106">ユーザーの分析に関する分析情報は、ユーザー環境分析のスコアを向上させるための推奨事項です。</span><span class="sxs-lookup"><span data-stu-id="eb477-106">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="eb477-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb477-107">Properties</span></span>
|<span data-ttu-id="eb477-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb477-108">Property</span></span>|<span data-ttu-id="eb477-109">型</span><span class="sxs-lookup"><span data-stu-id="eb477-109">Type</span></span>|<span data-ttu-id="eb477-110">説明</span><span class="sxs-lookup"><span data-stu-id="eb477-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb477-111">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="eb477-111">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="eb477-112">String</span><span class="sxs-lookup"><span data-stu-id="eb477-112">String</span></span>|<span data-ttu-id="eb477-113">ユーザー experience analytics に関する洞察の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="eb477-113">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="eb477-114">insightId</span><span class="sxs-lookup"><span data-stu-id="eb477-114">insightId</span></span>|<span data-ttu-id="eb477-115">String</span><span class="sxs-lookup"><span data-stu-id="eb477-115">String</span></span>|<span data-ttu-id="eb477-116">ユーザー experience analytics に関する洞察の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="eb477-116">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="eb477-117">value</span><span class="sxs-lookup"><span data-stu-id="eb477-117">value</span></span>|<span data-ttu-id="eb477-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="eb477-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="eb477-119">ユーザーが分析する分析に関する洞察の価値。</span><span class="sxs-lookup"><span data-stu-id="eb477-119">The value of the user experience analytics insight.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb477-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eb477-120">Relationships</span></span>
<span data-ttu-id="eb477-121">なし</span><span class="sxs-lookup"><span data-stu-id="eb477-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb477-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb477-122">JSON Representation</span></span>
<span data-ttu-id="eb477-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb477-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "userExperienceAnalyticsMetricId": "String",
  "insightId": "String",
  "value": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble"
    }
  ]
}
```



