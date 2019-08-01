---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5dd7ce37802e091489dfaeb4374bef087c951317
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028418"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="e62d3-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e62d3-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="e62d3-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e62d3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e62d3-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e62d3-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="e62d3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e62d3-106">Methods</span></span>
|<span data-ttu-id="e62d3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e62d3-107">Method</span></span>|<span data-ttu-id="e62d3-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e62d3-108">Return Type</span></span>|<span data-ttu-id="e62d3-109">説明</span><span class="sxs-lookup"><span data-stu-id="e62d3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e62d3-110">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e62d3-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="e62d3-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e62d3-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="e62d3-112">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e62d3-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="e62d3-113">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e62d3-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="e62d3-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e62d3-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="e62d3-115">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e62d3-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e62d3-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e62d3-116">Properties</span></span>
|<span data-ttu-id="e62d3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e62d3-117">Property</span></span>|<span data-ttu-id="e62d3-118">型</span><span class="sxs-lookup"><span data-stu-id="e62d3-118">Type</span></span>|<span data-ttu-id="e62d3-119">説明</span><span class="sxs-lookup"><span data-stu-id="e62d3-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e62d3-120">id</span><span class="sxs-lookup"><span data-stu-id="e62d3-120">id</span></span>|<span data-ttu-id="e62d3-121">String</span><span class="sxs-lookup"><span data-stu-id="e62d3-121">String</span></span>|<span data-ttu-id="e62d3-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e62d3-122">Key of the entity.</span></span>|
|<span data-ttu-id="e62d3-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e62d3-123">pendingCount</span></span>|<span data-ttu-id="e62d3-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e62d3-124">Int32</span></span>|<span data-ttu-id="e62d3-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e62d3-125">Number of pending Users</span></span>|
|<span data-ttu-id="e62d3-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e62d3-126">notApplicableCount</span></span>|<span data-ttu-id="e62d3-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e62d3-127">Int32</span></span>|<span data-ttu-id="e62d3-128">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e62d3-128">Number of not applicable users</span></span>|
|<span data-ttu-id="e62d3-129">successCount</span><span class="sxs-lookup"><span data-stu-id="e62d3-129">successCount</span></span>|<span data-ttu-id="e62d3-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e62d3-130">Int32</span></span>|<span data-ttu-id="e62d3-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e62d3-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="e62d3-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="e62d3-132">errorCount</span></span>|<span data-ttu-id="e62d3-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e62d3-133">Int32</span></span>|<span data-ttu-id="e62d3-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e62d3-134">Number of error Users</span></span>|
|<span data-ttu-id="e62d3-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="e62d3-135">failedCount</span></span>|<span data-ttu-id="e62d3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e62d3-136">Int32</span></span>|<span data-ttu-id="e62d3-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e62d3-137">Number of failed Users</span></span>|
|<span data-ttu-id="e62d3-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e62d3-138">lastUpdateDateTime</span></span>|<span data-ttu-id="e62d3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e62d3-139">DateTimeOffset</span></span>|<span data-ttu-id="e62d3-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="e62d3-140">Last update time</span></span>|
|<span data-ttu-id="e62d3-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e62d3-141">configurationVersion</span></span>|<span data-ttu-id="e62d3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e62d3-142">Int32</span></span>|<span data-ttu-id="e62d3-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="e62d3-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="e62d3-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e62d3-144">Relationships</span></span>
<span data-ttu-id="e62d3-145">なし</span><span class="sxs-lookup"><span data-stu-id="e62d3-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e62d3-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e62d3-146">JSON Representation</span></span>
<span data-ttu-id="e62d3-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e62d3-147">Here is a JSON representation of the resource.</span></span>
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



