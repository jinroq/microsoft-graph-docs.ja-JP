---
title: deviceConfigurationUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 74f56723702b50e855cc99f108950c708545fa5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303781"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="7e711-103">deviceConfigurationUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e711-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="7e711-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e711-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e711-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7e711-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="7e711-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e711-106">Methods</span></span>
|<span data-ttu-id="7e711-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e711-107">Method</span></span>|<span data-ttu-id="7e711-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7e711-108">Return Type</span></span>|<span data-ttu-id="7e711-109">説明</span><span class="sxs-lookup"><span data-stu-id="7e711-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e711-110">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7e711-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="7e711-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7e711-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="7e711-112">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7e711-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="7e711-113">Update deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7e711-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="7e711-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7e711-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="7e711-115">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7e711-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e711-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e711-116">Properties</span></span>
|<span data-ttu-id="7e711-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e711-117">Property</span></span>|<span data-ttu-id="7e711-118">種類</span><span class="sxs-lookup"><span data-stu-id="7e711-118">Type</span></span>|<span data-ttu-id="7e711-119">説明</span><span class="sxs-lookup"><span data-stu-id="7e711-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e711-120">ID</span><span class="sxs-lookup"><span data-stu-id="7e711-120">id</span></span>|<span data-ttu-id="7e711-121">String</span><span class="sxs-lookup"><span data-stu-id="7e711-121">String</span></span>|<span data-ttu-id="7e711-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7e711-122">Key of the entity.</span></span>|
|<span data-ttu-id="7e711-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="7e711-123">pendingCount</span></span>|<span data-ttu-id="7e711-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7e711-124">Int32</span></span>|<span data-ttu-id="7e711-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="7e711-125">Number of pending Users</span></span>|
|<span data-ttu-id="7e711-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="7e711-126">notApplicableCount</span></span>|<span data-ttu-id="7e711-127">Int32</span><span class="sxs-lookup"><span data-stu-id="7e711-127">Int32</span></span>|<span data-ttu-id="7e711-128">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="7e711-128">Number of not applicable users</span></span>|
|<span data-ttu-id="7e711-129">successCount</span><span class="sxs-lookup"><span data-stu-id="7e711-129">successCount</span></span>|<span data-ttu-id="7e711-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7e711-130">Int32</span></span>|<span data-ttu-id="7e711-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="7e711-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="7e711-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="7e711-132">errorCount</span></span>|<span data-ttu-id="7e711-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7e711-133">Int32</span></span>|<span data-ttu-id="7e711-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="7e711-134">Number of error Users</span></span>|
|<span data-ttu-id="7e711-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="7e711-135">failedCount</span></span>|<span data-ttu-id="7e711-136">Int32</span><span class="sxs-lookup"><span data-stu-id="7e711-136">Int32</span></span>|<span data-ttu-id="7e711-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="7e711-137">Number of failed Users</span></span>|
|<span data-ttu-id="7e711-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="7e711-138">lastUpdateDateTime</span></span>|<span data-ttu-id="7e711-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e711-139">DateTimeOffset</span></span>|<span data-ttu-id="7e711-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="7e711-140">Last update time</span></span>|
|<span data-ttu-id="7e711-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="7e711-141">configurationVersion</span></span>|<span data-ttu-id="7e711-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7e711-142">Int32</span></span>|<span data-ttu-id="7e711-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="7e711-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e711-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e711-144">Relationships</span></span>
<span data-ttu-id="7e711-145">なし</span><span class="sxs-lookup"><span data-stu-id="7e711-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e711-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e711-146">JSON Representation</span></span>
<span data-ttu-id="7e711-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e711-147">Here is a JSON representation of the resource.</span></span>
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



