---
title: managementCondition リソースの種類
description: 管理条件は、geo の囲いのように動的に発生することをイベントのタイム ・ フェンスとネットワーク フェンスです。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e0aeb73a93cd4c61b6d4680f73c2a9b8cee830c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986743"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="e0d7a-103">managementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0d7a-103">managementCondition resource type</span></span>

> <span data-ttu-id="e0d7a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0d7a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0d7a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0d7a-107">管理条件は、geo の囲いのように動的に発生することをイベントのタイム ・ フェンスとネットワーク フェンスです。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>
## <a name="methods"></a><span data-ttu-id="e0d7a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0d7a-108">Methods</span></span>
|<span data-ttu-id="e0d7a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0d7a-109">Method</span></span>|<span data-ttu-id="e0d7a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e0d7a-110">Return Type</span></span>|<span data-ttu-id="e0d7a-111">説明</span><span class="sxs-lookup"><span data-stu-id="e0d7a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0d7a-112">リスト managementConditions</span><span class="sxs-lookup"><span data-stu-id="e0d7a-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="e0d7a-113">[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e0d7a-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="e0d7a-114">[ManagementCondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="e0d7a-115">ManagementCondition を取得します。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="e0d7a-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="e0d7a-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="e0d7a-117">[ManagementCondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="e0d7a-118">getManagementConditionsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="e0d7a-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="e0d7a-119">[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e0d7a-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="e0d7a-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e0d7a-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e0d7a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0d7a-121">Properties</span></span>
|<span data-ttu-id="e0d7a-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0d7a-122">Property</span></span>|<span data-ttu-id="e0d7a-123">種類</span><span class="sxs-lookup"><span data-stu-id="e0d7a-123">Type</span></span>|<span data-ttu-id="e0d7a-124">説明</span><span class="sxs-lookup"><span data-stu-id="e0d7a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0d7a-125">ID</span><span class="sxs-lookup"><span data-stu-id="e0d7a-125">id</span></span>|<span data-ttu-id="e0d7a-126">String</span><span class="sxs-lookup"><span data-stu-id="e0d7a-126">String</span></span>|<span data-ttu-id="e0d7a-127">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="e0d7a-128">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="e0d7a-129">一意な名前</span><span class="sxs-lookup"><span data-stu-id="e0d7a-129">uniqueName</span></span>|<span data-ttu-id="e0d7a-130">String</span><span class="sxs-lookup"><span data-stu-id="e0d7a-130">String</span></span>|<span data-ttu-id="e0d7a-131">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-131">Unique name for the management condition.</span></span> <span data-ttu-id="e0d7a-132">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="e0d7a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e0d7a-133">displayName</span></span>|<span data-ttu-id="e0d7a-134">String</span><span class="sxs-lookup"><span data-stu-id="e0d7a-134">String</span></span>|<span data-ttu-id="e0d7a-135">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="e0d7a-136">説明</span><span class="sxs-lookup"><span data-stu-id="e0d7a-136">description</span></span>|<span data-ttu-id="e0d7a-137">String</span><span class="sxs-lookup"><span data-stu-id="e0d7a-137">String</span></span>|<span data-ttu-id="e0d7a-138">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="e0d7a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0d7a-139">createdDateTime</span></span>|<span data-ttu-id="e0d7a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0d7a-140">DateTimeOffset</span></span>|<span data-ttu-id="e0d7a-141">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-141">The time the management condition was created.</span></span> <span data-ttu-id="e0d7a-142">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-142">Generated service side.</span></span>|
|<span data-ttu-id="e0d7a-143">変更された日時</span><span class="sxs-lookup"><span data-stu-id="e0d7a-143">modifiedDateTime</span></span>|<span data-ttu-id="e0d7a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0d7a-144">DateTimeOffset</span></span>|<span data-ttu-id="e0d7a-145">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-145">The time the management condition was last modified.</span></span> <span data-ttu-id="e0d7a-146">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-146">Updated service side.</span></span>|
|<span data-ttu-id="e0d7a-147">eTag</span><span class="sxs-lookup"><span data-stu-id="e0d7a-147">eTag</span></span>|<span data-ttu-id="e0d7a-148">String</span><span class="sxs-lookup"><span data-stu-id="e0d7a-148">String</span></span>|<span data-ttu-id="e0d7a-149">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-149">ETag of the management condition.</span></span> <span data-ttu-id="e0d7a-150">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-150">Updated service side.</span></span>|
|<span data-ttu-id="e0d7a-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="e0d7a-151">applicablePlatforms</span></span>|<span data-ttu-id="e0d7a-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e0d7a-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="e0d7a-153">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0d7a-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0d7a-154">Relationships</span></span>
|<span data-ttu-id="e0d7a-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0d7a-155">Relationship</span></span>|<span data-ttu-id="e0d7a-156">型</span><span class="sxs-lookup"><span data-stu-id="e0d7a-156">Type</span></span>|<span data-ttu-id="e0d7a-157">説明</span><span class="sxs-lookup"><span data-stu-id="e0d7a-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0d7a-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="e0d7a-158">managementConditionStatements</span></span>|<span data-ttu-id="e0d7a-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e0d7a-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="e0d7a-160">管理条件に関連付けられている管理の条件ステートメントです。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0d7a-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0d7a-161">JSON Representation</span></span>
<span data-ttu-id="e0d7a-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0d7a-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





