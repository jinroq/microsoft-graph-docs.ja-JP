---
title: deviceConfigurationUserOverview リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02791ef66a387b80e0c84fa2473ad540fa662228
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995890"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="18884-103">deviceConfigurationUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18884-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="18884-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18884-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18884-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18884-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18884-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="18884-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="18884-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="18884-107">Methods</span></span>
|<span data-ttu-id="18884-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="18884-108">Method</span></span>|<span data-ttu-id="18884-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="18884-109">Return Type</span></span>|<span data-ttu-id="18884-110">説明</span><span class="sxs-lookup"><span data-stu-id="18884-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18884-111">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="18884-111">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="18884-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="18884-112">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="18884-113">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="18884-113">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="18884-114">Update deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="18884-114">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="18884-115">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="18884-115">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="18884-116">[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="18884-116">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18884-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18884-117">Properties</span></span>
|<span data-ttu-id="18884-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18884-118">Property</span></span>|<span data-ttu-id="18884-119">型</span><span class="sxs-lookup"><span data-stu-id="18884-119">Type</span></span>|<span data-ttu-id="18884-120">説明</span><span class="sxs-lookup"><span data-stu-id="18884-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18884-121">id</span><span class="sxs-lookup"><span data-stu-id="18884-121">id</span></span>|<span data-ttu-id="18884-122">String</span><span class="sxs-lookup"><span data-stu-id="18884-122">String</span></span>|<span data-ttu-id="18884-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="18884-123">Key of the entity.</span></span>|
|<span data-ttu-id="18884-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="18884-124">pendingCount</span></span>|<span data-ttu-id="18884-125">Int32</span><span class="sxs-lookup"><span data-stu-id="18884-125">Int32</span></span>|<span data-ttu-id="18884-126">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18884-126">Number of pending Users</span></span>|
|<span data-ttu-id="18884-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="18884-127">notApplicableCount</span></span>|<span data-ttu-id="18884-128">Int32</span><span class="sxs-lookup"><span data-stu-id="18884-128">Int32</span></span>|<span data-ttu-id="18884-129">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18884-129">Number of not applicable users</span></span>|
|<span data-ttu-id="18884-130">successCount</span><span class="sxs-lookup"><span data-stu-id="18884-130">successCount</span></span>|<span data-ttu-id="18884-131">Int32</span><span class="sxs-lookup"><span data-stu-id="18884-131">Int32</span></span>|<span data-ttu-id="18884-132">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18884-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="18884-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="18884-133">errorCount</span></span>|<span data-ttu-id="18884-134">Int32</span><span class="sxs-lookup"><span data-stu-id="18884-134">Int32</span></span>|<span data-ttu-id="18884-135">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18884-135">Number of error Users</span></span>|
|<span data-ttu-id="18884-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="18884-136">failedCount</span></span>|<span data-ttu-id="18884-137">Int32</span><span class="sxs-lookup"><span data-stu-id="18884-137">Int32</span></span>|<span data-ttu-id="18884-138">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18884-138">Number of failed Users</span></span>|
|<span data-ttu-id="18884-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="18884-139">conflictCount</span></span>|<span data-ttu-id="18884-140">Int32</span><span class="sxs-lookup"><span data-stu-id="18884-140">Int32</span></span>|<span data-ttu-id="18884-141">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18884-141">Number of users in conflict</span></span>|
|<span data-ttu-id="18884-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="18884-142">lastUpdateDateTime</span></span>|<span data-ttu-id="18884-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18884-143">DateTimeOffset</span></span>|<span data-ttu-id="18884-144">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="18884-144">Last update time</span></span>|
|<span data-ttu-id="18884-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="18884-145">configurationVersion</span></span>|<span data-ttu-id="18884-146">Int32</span><span class="sxs-lookup"><span data-stu-id="18884-146">Int32</span></span>|<span data-ttu-id="18884-147">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="18884-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="18884-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18884-148">Relationships</span></span>
<span data-ttu-id="18884-149">なし</span><span class="sxs-lookup"><span data-stu-id="18884-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18884-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18884-150">JSON Representation</span></span>
<span data-ttu-id="18884-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18884-151">Here is a JSON representation of the resource.</span></span>
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





