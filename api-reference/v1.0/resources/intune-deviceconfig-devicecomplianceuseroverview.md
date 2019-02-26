---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 177c66d9c09ce8ee1ac546e987e9475c5df3264f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260880"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="e3b92-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e3b92-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="e3b92-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3b92-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3b92-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e3b92-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="e3b92-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3b92-106">Methods</span></span>
|<span data-ttu-id="e3b92-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3b92-107">Method</span></span>|<span data-ttu-id="e3b92-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e3b92-108">Return Type</span></span>|<span data-ttu-id="e3b92-109">説明</span><span class="sxs-lookup"><span data-stu-id="e3b92-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3b92-110">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e3b92-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="e3b92-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e3b92-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="e3b92-112">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e3b92-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="e3b92-113">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e3b92-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="e3b92-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e3b92-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="e3b92-115">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3b92-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3b92-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3b92-116">Properties</span></span>
|<span data-ttu-id="e3b92-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3b92-117">Property</span></span>|<span data-ttu-id="e3b92-118">型</span><span class="sxs-lookup"><span data-stu-id="e3b92-118">Type</span></span>|<span data-ttu-id="e3b92-119">説明</span><span class="sxs-lookup"><span data-stu-id="e3b92-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3b92-120">id</span><span class="sxs-lookup"><span data-stu-id="e3b92-120">id</span></span>|<span data-ttu-id="e3b92-121">String</span><span class="sxs-lookup"><span data-stu-id="e3b92-121">String</span></span>|<span data-ttu-id="e3b92-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e3b92-122">Key of the entity.</span></span>|
|<span data-ttu-id="e3b92-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e3b92-123">pendingCount</span></span>|<span data-ttu-id="e3b92-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b92-124">Int32</span></span>|<span data-ttu-id="e3b92-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e3b92-125">Number of pending Users</span></span>|
|<span data-ttu-id="e3b92-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e3b92-126">notApplicableCount</span></span>|<span data-ttu-id="e3b92-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b92-127">Int32</span></span>|<span data-ttu-id="e3b92-128">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e3b92-128">Number of not applicable users</span></span>|
|<span data-ttu-id="e3b92-129">successCount</span><span class="sxs-lookup"><span data-stu-id="e3b92-129">successCount</span></span>|<span data-ttu-id="e3b92-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b92-130">Int32</span></span>|<span data-ttu-id="e3b92-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e3b92-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="e3b92-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="e3b92-132">errorCount</span></span>|<span data-ttu-id="e3b92-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b92-133">Int32</span></span>|<span data-ttu-id="e3b92-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e3b92-134">Number of error Users</span></span>|
|<span data-ttu-id="e3b92-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="e3b92-135">failedCount</span></span>|<span data-ttu-id="e3b92-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b92-136">Int32</span></span>|<span data-ttu-id="e3b92-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="e3b92-137">Number of failed Users</span></span>|
|<span data-ttu-id="e3b92-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e3b92-138">lastUpdateDateTime</span></span>|<span data-ttu-id="e3b92-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3b92-139">DateTimeOffset</span></span>|<span data-ttu-id="e3b92-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="e3b92-140">Last update time</span></span>|
|<span data-ttu-id="e3b92-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e3b92-141">configurationVersion</span></span>|<span data-ttu-id="e3b92-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b92-142">Int32</span></span>|<span data-ttu-id="e3b92-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="e3b92-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3b92-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3b92-144">Relationships</span></span>
<span data-ttu-id="e3b92-145">なし</span><span class="sxs-lookup"><span data-stu-id="e3b92-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3b92-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e3b92-146">JSON Representation</span></span>
<span data-ttu-id="e3b92-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e3b92-147">Here is a JSON representation of the resource.</span></span>
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



