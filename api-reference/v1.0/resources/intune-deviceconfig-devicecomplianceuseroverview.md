---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 01596e7b4e5c4d5a661befadbffa00529d3314d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973196"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="94c58-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="94c58-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="94c58-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="94c58-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94c58-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="94c58-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="94c58-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="94c58-106">Methods</span></span>
|<span data-ttu-id="94c58-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="94c58-107">Method</span></span>|<span data-ttu-id="94c58-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="94c58-108">Return Type</span></span>|<span data-ttu-id="94c58-109">説明</span><span class="sxs-lookup"><span data-stu-id="94c58-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94c58-110">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="94c58-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="94c58-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="94c58-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="94c58-112">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="94c58-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="94c58-113">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="94c58-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="94c58-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="94c58-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="94c58-115">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="94c58-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94c58-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94c58-116">Properties</span></span>
|<span data-ttu-id="94c58-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94c58-117">Property</span></span>|<span data-ttu-id="94c58-118">種類</span><span class="sxs-lookup"><span data-stu-id="94c58-118">Type</span></span>|<span data-ttu-id="94c58-119">説明</span><span class="sxs-lookup"><span data-stu-id="94c58-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94c58-120">ID</span><span class="sxs-lookup"><span data-stu-id="94c58-120">id</span></span>|<span data-ttu-id="94c58-121">String</span><span class="sxs-lookup"><span data-stu-id="94c58-121">String</span></span>|<span data-ttu-id="94c58-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="94c58-122">Key of the entity.</span></span>|
|<span data-ttu-id="94c58-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="94c58-123">pendingCount</span></span>|<span data-ttu-id="94c58-124">Int32</span><span class="sxs-lookup"><span data-stu-id="94c58-124">Int32</span></span>|<span data-ttu-id="94c58-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="94c58-125">Number of pending Users</span></span>|
|<span data-ttu-id="94c58-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="94c58-126">notApplicableCount</span></span>|<span data-ttu-id="94c58-127">Int32</span><span class="sxs-lookup"><span data-stu-id="94c58-127">Int32</span></span>|<span data-ttu-id="94c58-128">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="94c58-128">Number of not applicable users</span></span>|
|<span data-ttu-id="94c58-129">successCount</span><span class="sxs-lookup"><span data-stu-id="94c58-129">successCount</span></span>|<span data-ttu-id="94c58-130">Int32</span><span class="sxs-lookup"><span data-stu-id="94c58-130">Int32</span></span>|<span data-ttu-id="94c58-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="94c58-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="94c58-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="94c58-132">errorCount</span></span>|<span data-ttu-id="94c58-133">Int32</span><span class="sxs-lookup"><span data-stu-id="94c58-133">Int32</span></span>|<span data-ttu-id="94c58-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="94c58-134">Number of error Users</span></span>|
|<span data-ttu-id="94c58-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="94c58-135">failedCount</span></span>|<span data-ttu-id="94c58-136">Int32</span><span class="sxs-lookup"><span data-stu-id="94c58-136">Int32</span></span>|<span data-ttu-id="94c58-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="94c58-137">Number of failed Users</span></span>|
|<span data-ttu-id="94c58-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="94c58-138">lastUpdateDateTime</span></span>|<span data-ttu-id="94c58-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94c58-139">DateTimeOffset</span></span>|<span data-ttu-id="94c58-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="94c58-140">Last update time</span></span>|
|<span data-ttu-id="94c58-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="94c58-141">configurationVersion</span></span>|<span data-ttu-id="94c58-142">Int32</span><span class="sxs-lookup"><span data-stu-id="94c58-142">Int32</span></span>|<span data-ttu-id="94c58-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="94c58-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="94c58-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="94c58-144">Relationships</span></span>
<span data-ttu-id="94c58-145">なし</span><span class="sxs-lookup"><span data-stu-id="94c58-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94c58-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="94c58-146">JSON Representation</span></span>
<span data-ttu-id="94c58-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="94c58-147">Here is a JSON representation of the resource.</span></span>
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
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



