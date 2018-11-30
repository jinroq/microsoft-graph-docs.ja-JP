---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: ab4048bc8287c3ec225954c80009e69806480e4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072500"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="9b4eb-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b4eb-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="9b4eb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b4eb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b4eb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b4eb-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9b4eb-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="9b4eb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b4eb-108">Methods</span></span>
|<span data-ttu-id="9b4eb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b4eb-109">Method</span></span>|<span data-ttu-id="9b4eb-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9b4eb-110">Return Type</span></span>|<span data-ttu-id="9b4eb-111">説明</span><span class="sxs-lookup"><span data-stu-id="9b4eb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b4eb-112">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="9b4eb-112">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="9b4eb-113">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="9b4eb-113">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="9b4eb-114">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-114">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="9b4eb-115">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="9b4eb-115">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="9b4eb-116">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="9b4eb-116">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="9b4eb-117">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-117">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b4eb-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b4eb-118">Properties</span></span>
|<span data-ttu-id="9b4eb-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b4eb-119">Property</span></span>|<span data-ttu-id="9b4eb-120">型</span><span class="sxs-lookup"><span data-stu-id="9b4eb-120">Type</span></span>|<span data-ttu-id="9b4eb-121">説明</span><span class="sxs-lookup"><span data-stu-id="9b4eb-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b4eb-122">id</span><span class="sxs-lookup"><span data-stu-id="9b4eb-122">id</span></span>|<span data-ttu-id="9b4eb-123">String</span><span class="sxs-lookup"><span data-stu-id="9b4eb-123">String</span></span>|<span data-ttu-id="9b4eb-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-124">Key of the entity.</span></span>|
|<span data-ttu-id="9b4eb-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="9b4eb-125">pendingCount</span></span>|<span data-ttu-id="9b4eb-126">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4eb-126">Int32</span></span>|<span data-ttu-id="9b4eb-127">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b4eb-127">Number of pending Users</span></span>|
|<span data-ttu-id="9b4eb-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9b4eb-128">notApplicableCount</span></span>|<span data-ttu-id="9b4eb-129">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4eb-129">Int32</span></span>|<span data-ttu-id="9b4eb-130">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b4eb-130">Number of not applicable users</span></span>|
|<span data-ttu-id="9b4eb-131">successCount</span><span class="sxs-lookup"><span data-stu-id="9b4eb-131">successCount</span></span>|<span data-ttu-id="9b4eb-132">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4eb-132">Int32</span></span>|<span data-ttu-id="9b4eb-133">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b4eb-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="9b4eb-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="9b4eb-134">errorCount</span></span>|<span data-ttu-id="9b4eb-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4eb-135">Int32</span></span>|<span data-ttu-id="9b4eb-136">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b4eb-136">Number of error Users</span></span>|
|<span data-ttu-id="9b4eb-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="9b4eb-137">failedCount</span></span>|<span data-ttu-id="9b4eb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4eb-138">Int32</span></span>|<span data-ttu-id="9b4eb-139">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b4eb-139">Number of failed Users</span></span>|
|<span data-ttu-id="9b4eb-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9b4eb-140">conflictCount</span></span>|<span data-ttu-id="9b4eb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4eb-141">Int32</span></span>|<span data-ttu-id="9b4eb-142">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9b4eb-142">Number of users in conflict</span></span>|
|<span data-ttu-id="9b4eb-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9b4eb-143">lastUpdateDateTime</span></span>|<span data-ttu-id="9b4eb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b4eb-144">DateTimeOffset</span></span>|<span data-ttu-id="9b4eb-145">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="9b4eb-145">Last update time</span></span>|
|<span data-ttu-id="9b4eb-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="9b4eb-146">configurationVersion</span></span>|<span data-ttu-id="9b4eb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4eb-147">Int32</span></span>|<span data-ttu-id="9b4eb-148">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="9b4eb-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b4eb-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b4eb-149">Relationships</span></span>
<span data-ttu-id="9b4eb-150">なし</span><span class="sxs-lookup"><span data-stu-id="9b4eb-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b4eb-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b4eb-151">JSON Representation</span></span>
<span data-ttu-id="9b4eb-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-152">Here is a JSON representation of the resource.</span></span>
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





