---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48bc71ce27656d68ad291e86b0157723a304f937
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565507"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="f5f19-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5f19-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="f5f19-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5f19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5f19-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5f19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5f19-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f5f19-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="f5f19-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5f19-107">Methods</span></span>
|<span data-ttu-id="f5f19-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5f19-108">Method</span></span>|<span data-ttu-id="f5f19-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5f19-109">Return Type</span></span>|<span data-ttu-id="f5f19-110">説明</span><span class="sxs-lookup"><span data-stu-id="f5f19-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f5f19-111">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f5f19-111">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="f5f19-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f5f19-112">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="f5f19-113">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f5f19-113">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="f5f19-114">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f5f19-114">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="f5f19-115">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f5f19-115">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="f5f19-116">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f5f19-116">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5f19-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5f19-117">Properties</span></span>
|<span data-ttu-id="f5f19-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5f19-118">Property</span></span>|<span data-ttu-id="f5f19-119">型</span><span class="sxs-lookup"><span data-stu-id="f5f19-119">Type</span></span>|<span data-ttu-id="f5f19-120">説明</span><span class="sxs-lookup"><span data-stu-id="f5f19-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5f19-121">id</span><span class="sxs-lookup"><span data-stu-id="f5f19-121">id</span></span>|<span data-ttu-id="f5f19-122">String</span><span class="sxs-lookup"><span data-stu-id="f5f19-122">String</span></span>|<span data-ttu-id="f5f19-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f5f19-123">Key of the entity.</span></span>|
|<span data-ttu-id="f5f19-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f5f19-124">pendingCount</span></span>|<span data-ttu-id="f5f19-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f19-125">Int32</span></span>|<span data-ttu-id="f5f19-126">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f5f19-126">Number of pending Users</span></span>|
|<span data-ttu-id="f5f19-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f5f19-127">notApplicableCount</span></span>|<span data-ttu-id="f5f19-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f19-128">Int32</span></span>|<span data-ttu-id="f5f19-129">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f5f19-129">Number of not applicable users</span></span>|
|<span data-ttu-id="f5f19-130">successCount</span><span class="sxs-lookup"><span data-stu-id="f5f19-130">successCount</span></span>|<span data-ttu-id="f5f19-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f19-131">Int32</span></span>|<span data-ttu-id="f5f19-132">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f5f19-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="f5f19-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="f5f19-133">errorCount</span></span>|<span data-ttu-id="f5f19-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f19-134">Int32</span></span>|<span data-ttu-id="f5f19-135">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f5f19-135">Number of error Users</span></span>|
|<span data-ttu-id="f5f19-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="f5f19-136">failedCount</span></span>|<span data-ttu-id="f5f19-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f19-137">Int32</span></span>|<span data-ttu-id="f5f19-138">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f5f19-138">Number of failed Users</span></span>|
|<span data-ttu-id="f5f19-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="f5f19-139">conflictCount</span></span>|<span data-ttu-id="f5f19-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f19-140">Int32</span></span>|<span data-ttu-id="f5f19-141">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f5f19-141">Number of users in conflict</span></span>|
|<span data-ttu-id="f5f19-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f5f19-142">lastUpdateDateTime</span></span>|<span data-ttu-id="f5f19-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5f19-143">DateTimeOffset</span></span>|<span data-ttu-id="f5f19-144">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="f5f19-144">Last update time</span></span>|
|<span data-ttu-id="f5f19-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f5f19-145">configurationVersion</span></span>|<span data-ttu-id="f5f19-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f19-146">Int32</span></span>|<span data-ttu-id="f5f19-147">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="f5f19-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5f19-148">関係</span><span class="sxs-lookup"><span data-stu-id="f5f19-148">Relationships</span></span>
<span data-ttu-id="f5f19-149">なし</span><span class="sxs-lookup"><span data-stu-id="f5f19-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5f19-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5f19-150">JSON Representation</span></span>
<span data-ttu-id="f5f19-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5f19-151">Here is a JSON representation of the resource.</span></span>
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





