---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 177c66d9c09ce8ee1ac546e987e9475c5df3264f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567530"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="580bd-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="580bd-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="580bd-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="580bd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="580bd-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="580bd-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="580bd-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="580bd-106">Methods</span></span>
|<span data-ttu-id="580bd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="580bd-107">Method</span></span>|<span data-ttu-id="580bd-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="580bd-108">Return Type</span></span>|<span data-ttu-id="580bd-109">説明</span><span class="sxs-lookup"><span data-stu-id="580bd-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="580bd-110">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="580bd-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="580bd-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="580bd-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="580bd-112">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="580bd-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="580bd-113">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="580bd-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="580bd-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="580bd-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="580bd-115">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="580bd-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="580bd-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="580bd-116">Properties</span></span>
|<span data-ttu-id="580bd-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="580bd-117">Property</span></span>|<span data-ttu-id="580bd-118">型</span><span class="sxs-lookup"><span data-stu-id="580bd-118">Type</span></span>|<span data-ttu-id="580bd-119">説明</span><span class="sxs-lookup"><span data-stu-id="580bd-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="580bd-120">id</span><span class="sxs-lookup"><span data-stu-id="580bd-120">id</span></span>|<span data-ttu-id="580bd-121">String</span><span class="sxs-lookup"><span data-stu-id="580bd-121">String</span></span>|<span data-ttu-id="580bd-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="580bd-122">Key of the entity.</span></span>|
|<span data-ttu-id="580bd-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="580bd-123">pendingCount</span></span>|<span data-ttu-id="580bd-124">Int32</span><span class="sxs-lookup"><span data-stu-id="580bd-124">Int32</span></span>|<span data-ttu-id="580bd-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="580bd-125">Number of pending Users</span></span>|
|<span data-ttu-id="580bd-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="580bd-126">notApplicableCount</span></span>|<span data-ttu-id="580bd-127">Int32</span><span class="sxs-lookup"><span data-stu-id="580bd-127">Int32</span></span>|<span data-ttu-id="580bd-128">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="580bd-128">Number of not applicable users</span></span>|
|<span data-ttu-id="580bd-129">successCount</span><span class="sxs-lookup"><span data-stu-id="580bd-129">successCount</span></span>|<span data-ttu-id="580bd-130">Int32</span><span class="sxs-lookup"><span data-stu-id="580bd-130">Int32</span></span>|<span data-ttu-id="580bd-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="580bd-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="580bd-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="580bd-132">errorCount</span></span>|<span data-ttu-id="580bd-133">Int32</span><span class="sxs-lookup"><span data-stu-id="580bd-133">Int32</span></span>|<span data-ttu-id="580bd-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="580bd-134">Number of error Users</span></span>|
|<span data-ttu-id="580bd-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="580bd-135">failedCount</span></span>|<span data-ttu-id="580bd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="580bd-136">Int32</span></span>|<span data-ttu-id="580bd-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="580bd-137">Number of failed Users</span></span>|
|<span data-ttu-id="580bd-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="580bd-138">lastUpdateDateTime</span></span>|<span data-ttu-id="580bd-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="580bd-139">DateTimeOffset</span></span>|<span data-ttu-id="580bd-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="580bd-140">Last update time</span></span>|
|<span data-ttu-id="580bd-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="580bd-141">configurationVersion</span></span>|<span data-ttu-id="580bd-142">Int32</span><span class="sxs-lookup"><span data-stu-id="580bd-142">Int32</span></span>|<span data-ttu-id="580bd-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="580bd-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="580bd-144">関係</span><span class="sxs-lookup"><span data-stu-id="580bd-144">Relationships</span></span>
<span data-ttu-id="580bd-145">なし</span><span class="sxs-lookup"><span data-stu-id="580bd-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="580bd-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="580bd-146">JSON Representation</span></span>
<span data-ttu-id="580bd-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="580bd-147">Here is a JSON representation of the resource.</span></span>
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



