---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 112b366f9678d092b0a59699d9a9931376819eca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173424"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="0a46c-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a46c-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="0a46c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a46c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a46c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a46c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a46c-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0a46c-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="0a46c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a46c-107">Methods</span></span>
|<span data-ttu-id="0a46c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a46c-108">Method</span></span>|<span data-ttu-id="0a46c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0a46c-109">Return Type</span></span>|<span data-ttu-id="0a46c-110">説明</span><span class="sxs-lookup"><span data-stu-id="0a46c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0a46c-111">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="0a46c-111">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="0a46c-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="0a46c-112">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="0a46c-113">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0a46c-113">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="0a46c-114">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="0a46c-114">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="0a46c-115">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="0a46c-115">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="0a46c-116">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a46c-116">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0a46c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a46c-117">Properties</span></span>
|<span data-ttu-id="0a46c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a46c-118">Property</span></span>|<span data-ttu-id="0a46c-119">型</span><span class="sxs-lookup"><span data-stu-id="0a46c-119">Type</span></span>|<span data-ttu-id="0a46c-120">説明</span><span class="sxs-lookup"><span data-stu-id="0a46c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a46c-121">id</span><span class="sxs-lookup"><span data-stu-id="0a46c-121">id</span></span>|<span data-ttu-id="0a46c-122">String</span><span class="sxs-lookup"><span data-stu-id="0a46c-122">String</span></span>|<span data-ttu-id="0a46c-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0a46c-123">Key of the entity.</span></span>|
|<span data-ttu-id="0a46c-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0a46c-124">pendingCount</span></span>|<span data-ttu-id="0a46c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0a46c-125">Int32</span></span>|<span data-ttu-id="0a46c-126">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0a46c-126">Number of pending Users</span></span>|
|<span data-ttu-id="0a46c-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0a46c-127">notApplicableCount</span></span>|<span data-ttu-id="0a46c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0a46c-128">Int32</span></span>|<span data-ttu-id="0a46c-129">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0a46c-129">Number of not applicable users</span></span>|
|<span data-ttu-id="0a46c-130">successCount</span><span class="sxs-lookup"><span data-stu-id="0a46c-130">successCount</span></span>|<span data-ttu-id="0a46c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0a46c-131">Int32</span></span>|<span data-ttu-id="0a46c-132">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0a46c-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="0a46c-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="0a46c-133">errorCount</span></span>|<span data-ttu-id="0a46c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0a46c-134">Int32</span></span>|<span data-ttu-id="0a46c-135">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0a46c-135">Number of error Users</span></span>|
|<span data-ttu-id="0a46c-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="0a46c-136">failedCount</span></span>|<span data-ttu-id="0a46c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0a46c-137">Int32</span></span>|<span data-ttu-id="0a46c-138">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0a46c-138">Number of failed Users</span></span>|
|<span data-ttu-id="0a46c-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="0a46c-139">conflictCount</span></span>|<span data-ttu-id="0a46c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0a46c-140">Int32</span></span>|<span data-ttu-id="0a46c-141">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0a46c-141">Number of users in conflict</span></span>|
|<span data-ttu-id="0a46c-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0a46c-142">lastUpdateDateTime</span></span>|<span data-ttu-id="0a46c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a46c-143">DateTimeOffset</span></span>|<span data-ttu-id="0a46c-144">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="0a46c-144">Last update time</span></span>|
|<span data-ttu-id="0a46c-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0a46c-145">configurationVersion</span></span>|<span data-ttu-id="0a46c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0a46c-146">Int32</span></span>|<span data-ttu-id="0a46c-147">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="0a46c-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a46c-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a46c-148">Relationships</span></span>
<span data-ttu-id="0a46c-149">なし</span><span class="sxs-lookup"><span data-stu-id="0a46c-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a46c-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a46c-150">JSON Representation</span></span>
<span data-ttu-id="0a46c-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a46c-151">Here is a JSON representation of the resource.</span></span>
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




