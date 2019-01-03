---
title: deviceConfigurationUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: c844fd17e3287707a5ecacfb89c7b622497e2aac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310662"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="daeda-103">deviceConfigurationUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="daeda-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="daeda-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="daeda-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="daeda-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="daeda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="daeda-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="daeda-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="daeda-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="daeda-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="daeda-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="daeda-108">Methods</span></span>
|<span data-ttu-id="daeda-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="daeda-109">Method</span></span>|<span data-ttu-id="daeda-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="daeda-110">Return Type</span></span>|<span data-ttu-id="daeda-111">説明</span><span class="sxs-lookup"><span data-stu-id="daeda-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="daeda-112">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="daeda-112">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="daeda-113">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="daeda-113">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="daeda-114">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="daeda-114">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="daeda-115">Update deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="daeda-115">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="daeda-116">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="daeda-116">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="daeda-117">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="daeda-117">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="daeda-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="daeda-118">Properties</span></span>
|<span data-ttu-id="daeda-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="daeda-119">Property</span></span>|<span data-ttu-id="daeda-120">種類</span><span class="sxs-lookup"><span data-stu-id="daeda-120">Type</span></span>|<span data-ttu-id="daeda-121">説明</span><span class="sxs-lookup"><span data-stu-id="daeda-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daeda-122">ID</span><span class="sxs-lookup"><span data-stu-id="daeda-122">id</span></span>|<span data-ttu-id="daeda-123">String</span><span class="sxs-lookup"><span data-stu-id="daeda-123">String</span></span>|<span data-ttu-id="daeda-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="daeda-124">Key of the entity.</span></span>|
|<span data-ttu-id="daeda-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="daeda-125">pendingCount</span></span>|<span data-ttu-id="daeda-126">Int32</span><span class="sxs-lookup"><span data-stu-id="daeda-126">Int32</span></span>|<span data-ttu-id="daeda-127">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="daeda-127">Number of pending Users</span></span>|
|<span data-ttu-id="daeda-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="daeda-128">notApplicableCount</span></span>|<span data-ttu-id="daeda-129">Int32</span><span class="sxs-lookup"><span data-stu-id="daeda-129">Int32</span></span>|<span data-ttu-id="daeda-130">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="daeda-130">Number of not applicable users</span></span>|
|<span data-ttu-id="daeda-131">successCount</span><span class="sxs-lookup"><span data-stu-id="daeda-131">successCount</span></span>|<span data-ttu-id="daeda-132">Int32</span><span class="sxs-lookup"><span data-stu-id="daeda-132">Int32</span></span>|<span data-ttu-id="daeda-133">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="daeda-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="daeda-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="daeda-134">errorCount</span></span>|<span data-ttu-id="daeda-135">Int32</span><span class="sxs-lookup"><span data-stu-id="daeda-135">Int32</span></span>|<span data-ttu-id="daeda-136">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="daeda-136">Number of error Users</span></span>|
|<span data-ttu-id="daeda-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="daeda-137">failedCount</span></span>|<span data-ttu-id="daeda-138">Int32</span><span class="sxs-lookup"><span data-stu-id="daeda-138">Int32</span></span>|<span data-ttu-id="daeda-139">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="daeda-139">Number of failed Users</span></span>|
|<span data-ttu-id="daeda-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="daeda-140">conflictCount</span></span>|<span data-ttu-id="daeda-141">Int32</span><span class="sxs-lookup"><span data-stu-id="daeda-141">Int32</span></span>|<span data-ttu-id="daeda-142">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="daeda-142">Number of users in conflict</span></span>|
|<span data-ttu-id="daeda-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="daeda-143">lastUpdateDateTime</span></span>|<span data-ttu-id="daeda-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daeda-144">DateTimeOffset</span></span>|<span data-ttu-id="daeda-145">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="daeda-145">Last update time</span></span>|
|<span data-ttu-id="daeda-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="daeda-146">configurationVersion</span></span>|<span data-ttu-id="daeda-147">Int32</span><span class="sxs-lookup"><span data-stu-id="daeda-147">Int32</span></span>|<span data-ttu-id="daeda-148">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="daeda-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="daeda-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="daeda-149">Relationships</span></span>
<span data-ttu-id="daeda-150">なし</span><span class="sxs-lookup"><span data-stu-id="daeda-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="daeda-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="daeda-151">JSON Representation</span></span>
<span data-ttu-id="daeda-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="daeda-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
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




