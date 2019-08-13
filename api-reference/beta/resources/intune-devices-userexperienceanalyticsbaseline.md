---
title: userExperienceAnalyticsBaseline リソースの種類
description: User experience analytics baseline エンティティには、ユーザー experience analytics のスコアを比較するための基準値が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce77b448d381547bfc77b6a27e1e9935f252be5e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371528"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a><span data-ttu-id="ad566-103">userExperienceAnalyticsBaseline リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad566-103">userExperienceAnalyticsBaseline resource type</span></span>

> <span data-ttu-id="ad566-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad566-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad566-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad566-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad566-106">User experience analytics baseline エンティティには、ユーザー experience analytics のスコアを比較するための基準値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ad566-106">The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores.</span></span>

## <a name="methods"></a><span data-ttu-id="ad566-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad566-107">Methods</span></span>
|<span data-ttu-id="ad566-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad566-108">Method</span></span>|<span data-ttu-id="ad566-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ad566-109">Return Type</span></span>|<span data-ttu-id="ad566-110">説明</span><span class="sxs-lookup"><span data-stu-id="ad566-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ad566-111">リスト userExperienceAnalyticsBaselines</span><span class="sxs-lookup"><span data-stu-id="ad566-111">List userExperienceAnalyticsBaselines</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|<span data-ttu-id="ad566-112">[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ad566-112">[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) collection</span></span>|<span data-ttu-id="ad566-113">[UserExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ad566-113">List properties and relationships of the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) objects.</span></span>|
|[<span data-ttu-id="ad566-114">UserExperienceAnalyticsBaseline を取得する</span><span class="sxs-lookup"><span data-stu-id="ad566-114">Get userExperienceAnalyticsBaseline</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[<span data-ttu-id="ad566-115">userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="ad566-115">userExperienceAnalyticsBaseline</span></span>](../resources/intune-devices-userexperienceanalyticsbaseline.md)|<span data-ttu-id="ad566-116">[UserExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ad566-116">Read properties and relationships of the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>|
|[<span data-ttu-id="ad566-117">UserExperienceAnalyticsBaseline を作成する</span><span class="sxs-lookup"><span data-stu-id="ad566-117">Create userExperienceAnalyticsBaseline</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[<span data-ttu-id="ad566-118">userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="ad566-118">userExperienceAnalyticsBaseline</span></span>](../resources/intune-devices-userexperienceanalyticsbaseline.md)|<span data-ttu-id="ad566-119">新しい[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ad566-119">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>|
|[<span data-ttu-id="ad566-120">UserExperienceAnalyticsBaseline の削除</span><span class="sxs-lookup"><span data-stu-id="ad566-120">Delete userExperienceAnalyticsBaseline</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|<span data-ttu-id="ad566-121">None</span><span class="sxs-lookup"><span data-stu-id="ad566-121">None</span></span>|<span data-ttu-id="ad566-122">[UserExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="ad566-122">Deletes a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>|
|[<span data-ttu-id="ad566-123">UserExperienceAnalyticsBaseline の更新</span><span class="sxs-lookup"><span data-stu-id="ad566-123">Update userExperienceAnalyticsBaseline</span></span>](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[<span data-ttu-id="ad566-124">userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="ad566-124">userExperienceAnalyticsBaseline</span></span>](../resources/intune-devices-userexperienceanalyticsbaseline.md)|<span data-ttu-id="ad566-125">[UserExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ad566-125">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad566-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad566-126">Properties</span></span>
|<span data-ttu-id="ad566-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad566-127">Property</span></span>|<span data-ttu-id="ad566-128">型</span><span class="sxs-lookup"><span data-stu-id="ad566-128">Type</span></span>|<span data-ttu-id="ad566-129">説明</span><span class="sxs-lookup"><span data-stu-id="ad566-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad566-130">id</span><span class="sxs-lookup"><span data-stu-id="ad566-130">id</span></span>|<span data-ttu-id="ad566-131">文字列</span><span class="sxs-lookup"><span data-stu-id="ad566-131">String</span></span>|<span data-ttu-id="ad566-132">ユーザー experience analytics のベースラインの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="ad566-132">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="ad566-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ad566-133">displayName</span></span>|<span data-ttu-id="ad566-134">String</span><span class="sxs-lookup"><span data-stu-id="ad566-134">String</span></span>|<span data-ttu-id="ad566-135">ユーザー experience analytics のベースラインの名前。</span><span class="sxs-lookup"><span data-stu-id="ad566-135">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="ad566-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="ad566-136">overallScore</span></span>|<span data-ttu-id="ad566-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ad566-137">Int32</span></span>|<span data-ttu-id="ad566-138">ユーザー experience analytics のベースラインの全体的なスコア。</span><span class="sxs-lookup"><span data-stu-id="ad566-138">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="ad566-139">overallRegressionThreshold</span><span class="sxs-lookup"><span data-stu-id="ad566-139">overallRegressionThreshold</span></span>|<span data-ttu-id="ad566-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ad566-140">Int32</span></span>|<span data-ttu-id="ad566-141">ユーザー experience analytics のベースラインの全体的な回帰しきい値。</span><span class="sxs-lookup"><span data-stu-id="ad566-141">The overall regression threshold of the user experience analytics baseline.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad566-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad566-142">Relationships</span></span>
|<span data-ttu-id="ad566-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad566-143">Relationship</span></span>|<span data-ttu-id="ad566-144">型</span><span class="sxs-lookup"><span data-stu-id="ad566-144">Type</span></span>|<span data-ttu-id="ad566-145">説明</span><span class="sxs-lookup"><span data-stu-id="ad566-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad566-146">deviceBootPerformanceMetrics</span><span class="sxs-lookup"><span data-stu-id="ad566-146">deviceBootPerformanceMetrics</span></span>|[<span data-ttu-id="ad566-147">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ad566-147">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="ad566-148">ユーザー experience analytics デバイスのブートパフォーマンス指標。</span><span class="sxs-lookup"><span data-stu-id="ad566-148">The user experience analytics device boot performance metrics.</span></span>|
|<span data-ttu-id="ad566-149">bestPracticesMetrics</span><span class="sxs-lookup"><span data-stu-id="ad566-149">bestPracticesMetrics</span></span>|[<span data-ttu-id="ad566-150">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ad566-150">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="ad566-151">ユーザー操作分析のベストプラクティスの指標。</span><span class="sxs-lookup"><span data-stu-id="ad566-151">The user experience analytics best practices metrics.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad566-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad566-152">JSON Representation</span></span>
<span data-ttu-id="ad566-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ad566-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "overallRegressionThreshold": 1024
}
```



