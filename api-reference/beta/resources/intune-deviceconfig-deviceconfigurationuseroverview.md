---
title: deviceConfigurationUserOverview リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d157c6e03c7a4068a3f05399b972e1d48eedfb8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332919"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="c0325-103">deviceConfigurationUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0325-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="c0325-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0325-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0325-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0325-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0325-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c0325-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="c0325-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c0325-107">Methods</span></span>
|<span data-ttu-id="c0325-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c0325-108">Method</span></span>|<span data-ttu-id="c0325-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c0325-109">Return Type</span></span>|<span data-ttu-id="c0325-110">説明</span><span class="sxs-lookup"><span data-stu-id="c0325-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0325-111">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c0325-111">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="c0325-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c0325-112">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c0325-113">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c0325-113">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="c0325-114">Update deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c0325-114">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="c0325-115">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c0325-115">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c0325-116">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c0325-116">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0325-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0325-117">Properties</span></span>
|<span data-ttu-id="c0325-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0325-118">Property</span></span>|<span data-ttu-id="c0325-119">型</span><span class="sxs-lookup"><span data-stu-id="c0325-119">Type</span></span>|<span data-ttu-id="c0325-120">説明</span><span class="sxs-lookup"><span data-stu-id="c0325-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0325-121">id</span><span class="sxs-lookup"><span data-stu-id="c0325-121">id</span></span>|<span data-ttu-id="c0325-122">String</span><span class="sxs-lookup"><span data-stu-id="c0325-122">String</span></span>|<span data-ttu-id="c0325-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c0325-123">Key of the entity.</span></span>|
|<span data-ttu-id="c0325-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="c0325-124">pendingCount</span></span>|<span data-ttu-id="c0325-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c0325-125">Int32</span></span>|<span data-ttu-id="c0325-126">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c0325-126">Number of pending Users</span></span>|
|<span data-ttu-id="c0325-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c0325-127">notApplicableCount</span></span>|<span data-ttu-id="c0325-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c0325-128">Int32</span></span>|<span data-ttu-id="c0325-129">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c0325-129">Number of not applicable users</span></span>|
|<span data-ttu-id="c0325-130">successCount</span><span class="sxs-lookup"><span data-stu-id="c0325-130">successCount</span></span>|<span data-ttu-id="c0325-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c0325-131">Int32</span></span>|<span data-ttu-id="c0325-132">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c0325-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="c0325-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="c0325-133">errorCount</span></span>|<span data-ttu-id="c0325-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c0325-134">Int32</span></span>|<span data-ttu-id="c0325-135">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c0325-135">Number of error Users</span></span>|
|<span data-ttu-id="c0325-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="c0325-136">failedCount</span></span>|<span data-ttu-id="c0325-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c0325-137">Int32</span></span>|<span data-ttu-id="c0325-138">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c0325-138">Number of failed Users</span></span>|
|<span data-ttu-id="c0325-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c0325-139">conflictCount</span></span>|<span data-ttu-id="c0325-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c0325-140">Int32</span></span>|<span data-ttu-id="c0325-141">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c0325-141">Number of users in conflict</span></span>|
|<span data-ttu-id="c0325-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c0325-142">lastUpdateDateTime</span></span>|<span data-ttu-id="c0325-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0325-143">DateTimeOffset</span></span>|<span data-ttu-id="c0325-144">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="c0325-144">Last update time</span></span>|
|<span data-ttu-id="c0325-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="c0325-145">configurationVersion</span></span>|<span data-ttu-id="c0325-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c0325-146">Int32</span></span>|<span data-ttu-id="c0325-147">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="c0325-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0325-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0325-148">Relationships</span></span>
<span data-ttu-id="c0325-149">なし</span><span class="sxs-lookup"><span data-stu-id="c0325-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0325-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0325-150">JSON Representation</span></span>
<span data-ttu-id="c0325-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0325-151">Here is a JSON representation of the resource.</span></span>
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



