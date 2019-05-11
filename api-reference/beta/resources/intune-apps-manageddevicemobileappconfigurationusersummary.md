---
title: managedDeviceMobileAppConfigurationUserSummary リソースの種類
description: MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9b15a02f8293809d04dff472e40a86fda08f84a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950082"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="409ec-103">managedDeviceMobileAppConfigurationUserSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="409ec-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="409ec-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="409ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="409ec-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="409ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="409ec-106">MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="409ec-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="409ec-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="409ec-107">Methods</span></span>
|<span data-ttu-id="409ec-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="409ec-108">Method</span></span>|<span data-ttu-id="409ec-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="409ec-109">Return Type</span></span>|<span data-ttu-id="409ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="409ec-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="409ec-111">managedDeviceMobileAppConfigurationUserSummary の取得</span><span class="sxs-lookup"><span data-stu-id="409ec-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="409ec-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="409ec-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="409ec-113">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="409ec-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="409ec-114">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="409ec-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="409ec-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="409ec-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="409ec-116">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="409ec-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="409ec-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="409ec-117">Properties</span></span>
|<span data-ttu-id="409ec-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="409ec-118">Property</span></span>|<span data-ttu-id="409ec-119">型</span><span class="sxs-lookup"><span data-stu-id="409ec-119">Type</span></span>|<span data-ttu-id="409ec-120">説明</span><span class="sxs-lookup"><span data-stu-id="409ec-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="409ec-121">id</span><span class="sxs-lookup"><span data-stu-id="409ec-121">id</span></span>|<span data-ttu-id="409ec-122">String</span><span class="sxs-lookup"><span data-stu-id="409ec-122">String</span></span>|<span data-ttu-id="409ec-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="409ec-123">Key of the entity.</span></span>|
|<span data-ttu-id="409ec-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="409ec-124">pendingCount</span></span>|<span data-ttu-id="409ec-125">Int32</span><span class="sxs-lookup"><span data-stu-id="409ec-125">Int32</span></span>|<span data-ttu-id="409ec-126">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="409ec-126">Number of pending Users</span></span>|
|<span data-ttu-id="409ec-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="409ec-127">notApplicableCount</span></span>|<span data-ttu-id="409ec-128">Int32</span><span class="sxs-lookup"><span data-stu-id="409ec-128">Int32</span></span>|<span data-ttu-id="409ec-129">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="409ec-129">Number of not applicable users</span></span>|
|<span data-ttu-id="409ec-130">successCount</span><span class="sxs-lookup"><span data-stu-id="409ec-130">successCount</span></span>|<span data-ttu-id="409ec-131">Int32</span><span class="sxs-lookup"><span data-stu-id="409ec-131">Int32</span></span>|<span data-ttu-id="409ec-132">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="409ec-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="409ec-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="409ec-133">errorCount</span></span>|<span data-ttu-id="409ec-134">Int32</span><span class="sxs-lookup"><span data-stu-id="409ec-134">Int32</span></span>|<span data-ttu-id="409ec-135">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="409ec-135">Number of error Users</span></span>|
|<span data-ttu-id="409ec-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="409ec-136">failedCount</span></span>|<span data-ttu-id="409ec-137">Int32</span><span class="sxs-lookup"><span data-stu-id="409ec-137">Int32</span></span>|<span data-ttu-id="409ec-138">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="409ec-138">Number of failed Users</span></span>|
|<span data-ttu-id="409ec-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="409ec-139">conflictCount</span></span>|<span data-ttu-id="409ec-140">Int32</span><span class="sxs-lookup"><span data-stu-id="409ec-140">Int32</span></span>|<span data-ttu-id="409ec-141">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="409ec-141">Number of users in conflict</span></span>|
|<span data-ttu-id="409ec-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="409ec-142">lastUpdateDateTime</span></span>|<span data-ttu-id="409ec-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="409ec-143">DateTimeOffset</span></span>|<span data-ttu-id="409ec-144">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="409ec-144">Last update time</span></span>|
|<span data-ttu-id="409ec-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="409ec-145">configurationVersion</span></span>|<span data-ttu-id="409ec-146">Int32</span><span class="sxs-lookup"><span data-stu-id="409ec-146">Int32</span></span>|<span data-ttu-id="409ec-147">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="409ec-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="409ec-148">関係</span><span class="sxs-lookup"><span data-stu-id="409ec-148">Relationships</span></span>
<span data-ttu-id="409ec-149">なし</span><span class="sxs-lookup"><span data-stu-id="409ec-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="409ec-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="409ec-150">JSON Representation</span></span>
<span data-ttu-id="409ec-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="409ec-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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




