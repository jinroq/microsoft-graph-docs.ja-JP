---
title: softwareUpdateStatusSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cdc05c903f2e868dfadfb6ec4317aec0d1c9c4b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928228"
---
# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="0658a-103">softwareUpdateStatusSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0658a-103">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="0658a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0658a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0658a-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0658a-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="0658a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0658a-106">Methods</span></span>
|<span data-ttu-id="0658a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0658a-107">Method</span></span>|<span data-ttu-id="0658a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0658a-108">Return Type</span></span>|<span data-ttu-id="0658a-109">説明</span><span class="sxs-lookup"><span data-stu-id="0658a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0658a-110">Get softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0658a-110">Get softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[<span data-ttu-id="0658a-111">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0658a-111">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="0658a-112">[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0658a-112">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="0658a-113">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0658a-113">Update softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[<span data-ttu-id="0658a-114">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0658a-114">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="0658a-115">[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0658a-115">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0658a-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0658a-116">Properties</span></span>
|<span data-ttu-id="0658a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0658a-117">Property</span></span>|<span data-ttu-id="0658a-118">型</span><span class="sxs-lookup"><span data-stu-id="0658a-118">Type</span></span>|<span data-ttu-id="0658a-119">説明</span><span class="sxs-lookup"><span data-stu-id="0658a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0658a-120">ID</span><span class="sxs-lookup"><span data-stu-id="0658a-120">id</span></span>|<span data-ttu-id="0658a-121">String</span><span class="sxs-lookup"><span data-stu-id="0658a-121">String</span></span>|<span data-ttu-id="0658a-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0658a-122">Key of the entity.</span></span>|
|<span data-ttu-id="0658a-123">displayName</span><span class="sxs-lookup"><span data-stu-id="0658a-123">displayName</span></span>|<span data-ttu-id="0658a-124">String</span><span class="sxs-lookup"><span data-stu-id="0658a-124">String</span></span>|<span data-ttu-id="0658a-125">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="0658a-125">The name of the policy.</span></span>|
|<span data-ttu-id="0658a-126">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0658a-126">compliantDeviceCount</span></span>|<span data-ttu-id="0658a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-127">Int32</span></span>|<span data-ttu-id="0658a-128">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-128">Number of compliant devices.</span></span>|
|<span data-ttu-id="0658a-129">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0658a-129">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0658a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-130">Int32</span></span>|<span data-ttu-id="0658a-131">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-131">Number of non compliant devices.</span></span>|
|<span data-ttu-id="0658a-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0658a-132">remediatedDeviceCount</span></span>|<span data-ttu-id="0658a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-133">Int32</span></span>|<span data-ttu-id="0658a-134">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-134">Number of remediated devices.</span></span>|
|<span data-ttu-id="0658a-135">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0658a-135">errorDeviceCount</span></span>|<span data-ttu-id="0658a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-136">Int32</span></span>|<span data-ttu-id="0658a-137">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-137">Number of devices had error.</span></span>|
|<span data-ttu-id="0658a-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0658a-138">unknownDeviceCount</span></span>|<span data-ttu-id="0658a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-139">Int32</span></span>|<span data-ttu-id="0658a-140">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-140">Number of unknown devices.</span></span>|
|<span data-ttu-id="0658a-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0658a-141">conflictDeviceCount</span></span>|<span data-ttu-id="0658a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-142">Int32</span></span>|<span data-ttu-id="0658a-143">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-143">Number of conflict devices.</span></span>|
|<span data-ttu-id="0658a-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0658a-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="0658a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-145">Int32</span></span>|<span data-ttu-id="0658a-146">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-146">Number of not applicable devices.</span></span>|
|<span data-ttu-id="0658a-147">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="0658a-147">compliantUserCount</span></span>|<span data-ttu-id="0658a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-148">Int32</span></span>|<span data-ttu-id="0658a-149">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-149">Number of compliant users.</span></span>|
|<span data-ttu-id="0658a-150">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="0658a-150">nonCompliantUserCount</span></span>|<span data-ttu-id="0658a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-151">Int32</span></span>|<span data-ttu-id="0658a-152">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-152">Number of non compliant users.</span></span>|
|<span data-ttu-id="0658a-153">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="0658a-153">remediatedUserCount</span></span>|<span data-ttu-id="0658a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-154">Int32</span></span>|<span data-ttu-id="0658a-155">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-155">Number of remediated users.</span></span>|
|<span data-ttu-id="0658a-156">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="0658a-156">errorUserCount</span></span>|<span data-ttu-id="0658a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-157">Int32</span></span>|<span data-ttu-id="0658a-158">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-158">Number of users had error.</span></span>|
|<span data-ttu-id="0658a-159">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="0658a-159">unknownUserCount</span></span>|<span data-ttu-id="0658a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-160">Int32</span></span>|<span data-ttu-id="0658a-161">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-161">Number of unknown users.</span></span>|
|<span data-ttu-id="0658a-162">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="0658a-162">conflictUserCount</span></span>|<span data-ttu-id="0658a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-163">Int32</span></span>|<span data-ttu-id="0658a-164">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-164">Number of conflict users.</span></span>|
|<span data-ttu-id="0658a-165">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="0658a-165">notApplicableUserCount</span></span>|<span data-ttu-id="0658a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="0658a-166">Int32</span></span>|<span data-ttu-id="0658a-167">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="0658a-167">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0658a-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0658a-168">Relationships</span></span>
<span data-ttu-id="0658a-169">なし</span><span class="sxs-lookup"><span data-stu-id="0658a-169">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0658a-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0658a-170">JSON Representation</span></span>
<span data-ttu-id="0658a-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0658a-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```



