---
title: deviceComplianceUserOverview リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ec9228ce8e762a377cedac7258491f8ae34ef9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970487"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="00682-103">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="00682-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="00682-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00682-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00682-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="00682-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00682-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="00682-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="00682-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="00682-107">Methods</span></span>
|<span data-ttu-id="00682-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="00682-108">Method</span></span>|<span data-ttu-id="00682-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="00682-109">Return Type</span></span>|<span data-ttu-id="00682-110">説明</span><span class="sxs-lookup"><span data-stu-id="00682-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00682-111">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="00682-111">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="00682-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="00682-112">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="00682-113">[deviceCategory](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="00682-113">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="00682-114">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="00682-114">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="00682-115">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="00682-115">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="00682-116">[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="00682-116">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00682-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00682-117">Properties</span></span>
|<span data-ttu-id="00682-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00682-118">Property</span></span>|<span data-ttu-id="00682-119">型</span><span class="sxs-lookup"><span data-stu-id="00682-119">Type</span></span>|<span data-ttu-id="00682-120">説明</span><span class="sxs-lookup"><span data-stu-id="00682-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00682-121">id</span><span class="sxs-lookup"><span data-stu-id="00682-121">id</span></span>|<span data-ttu-id="00682-122">String</span><span class="sxs-lookup"><span data-stu-id="00682-122">String</span></span>|<span data-ttu-id="00682-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="00682-123">Key of the entity.</span></span>|
|<span data-ttu-id="00682-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="00682-124">pendingCount</span></span>|<span data-ttu-id="00682-125">Int32</span><span class="sxs-lookup"><span data-stu-id="00682-125">Int32</span></span>|<span data-ttu-id="00682-126">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="00682-126">Number of pending Users</span></span>|
|<span data-ttu-id="00682-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="00682-127">notApplicableCount</span></span>|<span data-ttu-id="00682-128">Int32</span><span class="sxs-lookup"><span data-stu-id="00682-128">Int32</span></span>|<span data-ttu-id="00682-129">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="00682-129">Number of not applicable users</span></span>|
|<span data-ttu-id="00682-130">successCount</span><span class="sxs-lookup"><span data-stu-id="00682-130">successCount</span></span>|<span data-ttu-id="00682-131">Int32</span><span class="sxs-lookup"><span data-stu-id="00682-131">Int32</span></span>|<span data-ttu-id="00682-132">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="00682-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="00682-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="00682-133">errorCount</span></span>|<span data-ttu-id="00682-134">Int32</span><span class="sxs-lookup"><span data-stu-id="00682-134">Int32</span></span>|<span data-ttu-id="00682-135">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="00682-135">Number of error Users</span></span>|
|<span data-ttu-id="00682-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="00682-136">failedCount</span></span>|<span data-ttu-id="00682-137">Int32</span><span class="sxs-lookup"><span data-stu-id="00682-137">Int32</span></span>|<span data-ttu-id="00682-138">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="00682-138">Number of failed Users</span></span>|
|<span data-ttu-id="00682-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="00682-139">conflictCount</span></span>|<span data-ttu-id="00682-140">Int32</span><span class="sxs-lookup"><span data-stu-id="00682-140">Int32</span></span>|<span data-ttu-id="00682-141">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="00682-141">Number of users in conflict</span></span>|
|<span data-ttu-id="00682-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="00682-142">lastUpdateDateTime</span></span>|<span data-ttu-id="00682-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00682-143">DateTimeOffset</span></span>|<span data-ttu-id="00682-144">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="00682-144">Last update time</span></span>|
|<span data-ttu-id="00682-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="00682-145">configurationVersion</span></span>|<span data-ttu-id="00682-146">Int32</span><span class="sxs-lookup"><span data-stu-id="00682-146">Int32</span></span>|<span data-ttu-id="00682-147">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="00682-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="00682-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="00682-148">Relationships</span></span>
<span data-ttu-id="00682-149">なし</span><span class="sxs-lookup"><span data-stu-id="00682-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00682-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00682-150">JSON Representation</span></span>
<span data-ttu-id="00682-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="00682-151">Here is a JSON representation of the resource.</span></span>
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





