---
title: deviceConfigurationUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0103d6eda14e2411a3ece16a7dcff8eef50d9b9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883973"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="1ed5d-103">deviceConfigurationUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1ed5d-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="1ed5d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ed5d-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1ed5d-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="1ed5d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1ed5d-106">Methods</span></span>
|<span data-ttu-id="1ed5d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1ed5d-107">Method</span></span>|<span data-ttu-id="1ed5d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1ed5d-108">Return Type</span></span>|<span data-ttu-id="1ed5d-109">説明</span><span class="sxs-lookup"><span data-stu-id="1ed5d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1ed5d-110">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1ed5d-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="1ed5d-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1ed5d-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1ed5d-112">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="1ed5d-113">Update deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1ed5d-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="1ed5d-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1ed5d-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1ed5d-115">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ed5d-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-116">Properties</span></span>
|<span data-ttu-id="1ed5d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-117">Property</span></span>|<span data-ttu-id="1ed5d-118">種類</span><span class="sxs-lookup"><span data-stu-id="1ed5d-118">Type</span></span>|<span data-ttu-id="1ed5d-119">説明</span><span class="sxs-lookup"><span data-stu-id="1ed5d-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed5d-120">ID</span><span class="sxs-lookup"><span data-stu-id="1ed5d-120">id</span></span>|<span data-ttu-id="1ed5d-121">String</span><span class="sxs-lookup"><span data-stu-id="1ed5d-121">String</span></span>|<span data-ttu-id="1ed5d-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-122">Key of the entity.</span></span>|
|<span data-ttu-id="1ed5d-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="1ed5d-123">pendingCount</span></span>|<span data-ttu-id="1ed5d-124">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed5d-124">Int32</span></span>|<span data-ttu-id="1ed5d-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="1ed5d-125">Number of pending Users</span></span>|
|<span data-ttu-id="1ed5d-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1ed5d-126">notApplicableCount</span></span>|<span data-ttu-id="1ed5d-127">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed5d-127">Int32</span></span>|<span data-ttu-id="1ed5d-128">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="1ed5d-128">Number of not applicable users</span></span>|
|<span data-ttu-id="1ed5d-129">successCount</span><span class="sxs-lookup"><span data-stu-id="1ed5d-129">successCount</span></span>|<span data-ttu-id="1ed5d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed5d-130">Int32</span></span>|<span data-ttu-id="1ed5d-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="1ed5d-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="1ed5d-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="1ed5d-132">errorCount</span></span>|<span data-ttu-id="1ed5d-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed5d-133">Int32</span></span>|<span data-ttu-id="1ed5d-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="1ed5d-134">Number of error Users</span></span>|
|<span data-ttu-id="1ed5d-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="1ed5d-135">failedCount</span></span>|<span data-ttu-id="1ed5d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed5d-136">Int32</span></span>|<span data-ttu-id="1ed5d-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="1ed5d-137">Number of failed Users</span></span>|
|<span data-ttu-id="1ed5d-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1ed5d-138">lastUpdateDateTime</span></span>|<span data-ttu-id="1ed5d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ed5d-139">DateTimeOffset</span></span>|<span data-ttu-id="1ed5d-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="1ed5d-140">Last update time</span></span>|
|<span data-ttu-id="1ed5d-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="1ed5d-141">configurationVersion</span></span>|<span data-ttu-id="1ed5d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed5d-142">Int32</span></span>|<span data-ttu-id="1ed5d-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="1ed5d-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ed5d-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ed5d-144">Relationships</span></span>
<span data-ttu-id="1ed5d-145">なし</span><span class="sxs-lookup"><span data-stu-id="1ed5d-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ed5d-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ed5d-146">JSON Representation</span></span>
<span data-ttu-id="1ed5d-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1ed5d-147">Here is a JSON representation of the resource.</span></span>
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
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



