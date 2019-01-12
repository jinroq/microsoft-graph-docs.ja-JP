---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e7ef2f9283ec55169096f519f40b4764b6f307a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944181"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="03a00-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03a00-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="03a00-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="03a00-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03a00-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03a00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03a00-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="03a00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03a00-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="03a00-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="03a00-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="03a00-108">Methods</span></span>
|<span data-ttu-id="03a00-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="03a00-109">Method</span></span>|<span data-ttu-id="03a00-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="03a00-110">Return Type</span></span>|<span data-ttu-id="03a00-111">説明</span><span class="sxs-lookup"><span data-stu-id="03a00-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03a00-112">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="03a00-112">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="03a00-113">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="03a00-113">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="03a00-114">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="03a00-114">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="03a00-115">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="03a00-115">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="03a00-116">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="03a00-116">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="03a00-117">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="03a00-117">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="03a00-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03a00-118">Properties</span></span>
|<span data-ttu-id="03a00-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03a00-119">Property</span></span>|<span data-ttu-id="03a00-120">型</span><span class="sxs-lookup"><span data-stu-id="03a00-120">Type</span></span>|<span data-ttu-id="03a00-121">説明</span><span class="sxs-lookup"><span data-stu-id="03a00-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03a00-122">ID</span><span class="sxs-lookup"><span data-stu-id="03a00-122">id</span></span>|<span data-ttu-id="03a00-123">String</span><span class="sxs-lookup"><span data-stu-id="03a00-123">String</span></span>|<span data-ttu-id="03a00-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="03a00-124">Key of the entity.</span></span>|
|<span data-ttu-id="03a00-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="03a00-125">pendingCount</span></span>|<span data-ttu-id="03a00-126">Int32</span><span class="sxs-lookup"><span data-stu-id="03a00-126">Int32</span></span>|<span data-ttu-id="03a00-127">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="03a00-127">Number of pending Users</span></span>|
|<span data-ttu-id="03a00-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="03a00-128">notApplicableCount</span></span>|<span data-ttu-id="03a00-129">Int32</span><span class="sxs-lookup"><span data-stu-id="03a00-129">Int32</span></span>|<span data-ttu-id="03a00-130">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="03a00-130">Number of not applicable users</span></span>|
|<span data-ttu-id="03a00-131">successCount</span><span class="sxs-lookup"><span data-stu-id="03a00-131">successCount</span></span>|<span data-ttu-id="03a00-132">Int32</span><span class="sxs-lookup"><span data-stu-id="03a00-132">Int32</span></span>|<span data-ttu-id="03a00-133">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="03a00-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="03a00-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="03a00-134">errorCount</span></span>|<span data-ttu-id="03a00-135">Int32</span><span class="sxs-lookup"><span data-stu-id="03a00-135">Int32</span></span>|<span data-ttu-id="03a00-136">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="03a00-136">Number of error Users</span></span>|
|<span data-ttu-id="03a00-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="03a00-137">failedCount</span></span>|<span data-ttu-id="03a00-138">Int32</span><span class="sxs-lookup"><span data-stu-id="03a00-138">Int32</span></span>|<span data-ttu-id="03a00-139">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="03a00-139">Number of failed Users</span></span>|
|<span data-ttu-id="03a00-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="03a00-140">conflictCount</span></span>|<span data-ttu-id="03a00-141">Int32</span><span class="sxs-lookup"><span data-stu-id="03a00-141">Int32</span></span>|<span data-ttu-id="03a00-142">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="03a00-142">Number of users in conflict</span></span>|
|<span data-ttu-id="03a00-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="03a00-143">lastUpdateDateTime</span></span>|<span data-ttu-id="03a00-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03a00-144">DateTimeOffset</span></span>|<span data-ttu-id="03a00-145">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="03a00-145">Last update time</span></span>|
|<span data-ttu-id="03a00-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="03a00-146">configurationVersion</span></span>|<span data-ttu-id="03a00-147">Int32</span><span class="sxs-lookup"><span data-stu-id="03a00-147">Int32</span></span>|<span data-ttu-id="03a00-148">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="03a00-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="03a00-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="03a00-149">Relationships</span></span>
<span data-ttu-id="03a00-150">なし</span><span class="sxs-lookup"><span data-stu-id="03a00-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03a00-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03a00-151">JSON Representation</span></span>
<span data-ttu-id="03a00-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="03a00-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





