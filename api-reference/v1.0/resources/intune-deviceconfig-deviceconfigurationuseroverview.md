---
title: deviceConfigurationUserOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ffae3151ee98bdef06b57a5ac9548735fefc5f2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028407"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="d7f31-103">deviceConfigurationUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7f31-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="d7f31-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7f31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7f31-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d7f31-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="d7f31-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7f31-106">Methods</span></span>
|<span data-ttu-id="d7f31-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7f31-107">Method</span></span>|<span data-ttu-id="d7f31-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d7f31-108">Return Type</span></span>|<span data-ttu-id="d7f31-109">説明</span><span class="sxs-lookup"><span data-stu-id="d7f31-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d7f31-110">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d7f31-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="d7f31-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d7f31-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="d7f31-112">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d7f31-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="d7f31-113">Update deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d7f31-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="d7f31-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d7f31-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="d7f31-115">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d7f31-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7f31-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7f31-116">Properties</span></span>
|<span data-ttu-id="d7f31-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7f31-117">Property</span></span>|<span data-ttu-id="d7f31-118">型</span><span class="sxs-lookup"><span data-stu-id="d7f31-118">Type</span></span>|<span data-ttu-id="d7f31-119">説明</span><span class="sxs-lookup"><span data-stu-id="d7f31-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7f31-120">id</span><span class="sxs-lookup"><span data-stu-id="d7f31-120">id</span></span>|<span data-ttu-id="d7f31-121">String</span><span class="sxs-lookup"><span data-stu-id="d7f31-121">String</span></span>|<span data-ttu-id="d7f31-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d7f31-122">Key of the entity.</span></span>|
|<span data-ttu-id="d7f31-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d7f31-123">pendingCount</span></span>|<span data-ttu-id="d7f31-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d7f31-124">Int32</span></span>|<span data-ttu-id="d7f31-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d7f31-125">Number of pending Users</span></span>|
|<span data-ttu-id="d7f31-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d7f31-126">notApplicableCount</span></span>|<span data-ttu-id="d7f31-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d7f31-127">Int32</span></span>|<span data-ttu-id="d7f31-128">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d7f31-128">Number of not applicable users</span></span>|
|<span data-ttu-id="d7f31-129">successCount</span><span class="sxs-lookup"><span data-stu-id="d7f31-129">successCount</span></span>|<span data-ttu-id="d7f31-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d7f31-130">Int32</span></span>|<span data-ttu-id="d7f31-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d7f31-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="d7f31-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="d7f31-132">errorCount</span></span>|<span data-ttu-id="d7f31-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d7f31-133">Int32</span></span>|<span data-ttu-id="d7f31-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d7f31-134">Number of error Users</span></span>|
|<span data-ttu-id="d7f31-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="d7f31-135">failedCount</span></span>|<span data-ttu-id="d7f31-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d7f31-136">Int32</span></span>|<span data-ttu-id="d7f31-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d7f31-137">Number of failed Users</span></span>|
|<span data-ttu-id="d7f31-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d7f31-138">lastUpdateDateTime</span></span>|<span data-ttu-id="d7f31-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7f31-139">DateTimeOffset</span></span>|<span data-ttu-id="d7f31-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="d7f31-140">Last update time</span></span>|
|<span data-ttu-id="d7f31-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d7f31-141">configurationVersion</span></span>|<span data-ttu-id="d7f31-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d7f31-142">Int32</span></span>|<span data-ttu-id="d7f31-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="d7f31-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7f31-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7f31-144">Relationships</span></span>
<span data-ttu-id="d7f31-145">なし</span><span class="sxs-lookup"><span data-stu-id="d7f31-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7f31-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7f31-146">JSON Representation</span></span>
<span data-ttu-id="d7f31-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d7f31-147">Here is a JSON representation of the resource.</span></span>
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



