---
title: managementCondition リソースの種類
description: 管理条件は、geo の囲いのように動的に発生することをイベントのタイム ・ フェンスとネットワーク フェンスです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c41b4cb3143349ba0fdd97633a70ec7b38e266ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405857"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="bb194-103">managementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb194-103">managementCondition resource type</span></span>

> <span data-ttu-id="bb194-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bb194-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb194-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb194-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb194-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb194-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb194-107">管理条件は、geo の囲いのように動的に発生することをイベントのタイム ・ フェンスとネットワーク フェンスです。</span><span class="sxs-lookup"><span data-stu-id="bb194-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="bb194-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb194-108">Methods</span></span>
|<span data-ttu-id="bb194-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb194-109">Method</span></span>|<span data-ttu-id="bb194-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb194-110">Return Type</span></span>|<span data-ttu-id="bb194-111">説明</span><span class="sxs-lookup"><span data-stu-id="bb194-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb194-112">リスト managementConditions</span><span class="sxs-lookup"><span data-stu-id="bb194-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="bb194-113">[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb194-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="bb194-114">[ManagementCondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bb194-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="bb194-115">ManagementCondition を取得します。</span><span class="sxs-lookup"><span data-stu-id="bb194-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="bb194-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="bb194-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="bb194-117">[ManagementCondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb194-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="bb194-118">getManagementConditionsForPlatform 関数</span><span class="sxs-lookup"><span data-stu-id="bb194-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="bb194-119">[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb194-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="bb194-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bb194-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bb194-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb194-121">Properties</span></span>
|<span data-ttu-id="bb194-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb194-122">Property</span></span>|<span data-ttu-id="bb194-123">型</span><span class="sxs-lookup"><span data-stu-id="bb194-123">Type</span></span>|<span data-ttu-id="bb194-124">説明</span><span class="sxs-lookup"><span data-stu-id="bb194-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb194-125">id</span><span class="sxs-lookup"><span data-stu-id="bb194-125">id</span></span>|<span data-ttu-id="bb194-126">String</span><span class="sxs-lookup"><span data-stu-id="bb194-126">String</span></span>|<span data-ttu-id="bb194-127">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="bb194-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="bb194-128">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="bb194-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="bb194-129">一意な名前</span><span class="sxs-lookup"><span data-stu-id="bb194-129">uniqueName</span></span>|<span data-ttu-id="bb194-130">String</span><span class="sxs-lookup"><span data-stu-id="bb194-130">String</span></span>|<span data-ttu-id="bb194-131">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="bb194-131">Unique name for the management condition.</span></span> <span data-ttu-id="bb194-132">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="bb194-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="bb194-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bb194-133">displayName</span></span>|<span data-ttu-id="bb194-134">String</span><span class="sxs-lookup"><span data-stu-id="bb194-134">String</span></span>|<span data-ttu-id="bb194-135">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="bb194-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="bb194-136">説明</span><span class="sxs-lookup"><span data-stu-id="bb194-136">description</span></span>|<span data-ttu-id="bb194-137">String</span><span class="sxs-lookup"><span data-stu-id="bb194-137">String</span></span>|<span data-ttu-id="bb194-138">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="bb194-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="bb194-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb194-139">createdDateTime</span></span>|<span data-ttu-id="bb194-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb194-140">DateTimeOffset</span></span>|<span data-ttu-id="bb194-141">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="bb194-141">The time the management condition was created.</span></span> <span data-ttu-id="bb194-142">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="bb194-142">Generated service side.</span></span>|
|<span data-ttu-id="bb194-143">変更された日時</span><span class="sxs-lookup"><span data-stu-id="bb194-143">modifiedDateTime</span></span>|<span data-ttu-id="bb194-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb194-144">DateTimeOffset</span></span>|<span data-ttu-id="bb194-145">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="bb194-145">The time the management condition was last modified.</span></span> <span data-ttu-id="bb194-146">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb194-146">Updated service side.</span></span>|
|<span data-ttu-id="bb194-147">eTag</span><span class="sxs-lookup"><span data-stu-id="bb194-147">eTag</span></span>|<span data-ttu-id="bb194-148">String</span><span class="sxs-lookup"><span data-stu-id="bb194-148">String</span></span>|<span data-ttu-id="bb194-149">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="bb194-149">ETag of the management condition.</span></span> <span data-ttu-id="bb194-150">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb194-150">Updated service side.</span></span>|
|<span data-ttu-id="bb194-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="bb194-151">applicablePlatforms</span></span>|<span data-ttu-id="bb194-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb194-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="bb194-153">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="bb194-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb194-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb194-154">Relationships</span></span>
|<span data-ttu-id="bb194-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb194-155">Relationship</span></span>|<span data-ttu-id="bb194-156">型</span><span class="sxs-lookup"><span data-stu-id="bb194-156">Type</span></span>|<span data-ttu-id="bb194-157">説明</span><span class="sxs-lookup"><span data-stu-id="bb194-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb194-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="bb194-158">managementConditionStatements</span></span>|<span data-ttu-id="bb194-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb194-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="bb194-160">管理条件に関連付けられている管理の条件ステートメントです。</span><span class="sxs-lookup"><span data-stu-id="bb194-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb194-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb194-161">JSON Representation</span></span>
<span data-ttu-id="bb194-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb194-162">Here is a JSON representation of the resource.</span></span>
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




