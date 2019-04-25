---
title: managedDeviceMobileAppConfigurationDeviceSummary リソースの種類
description: MDM モバイル アプリ構成のデバイス状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e62d02b5b702b56d72a0c75f9e5da1f6ad9dbdc3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583936"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="41e11-103">managedDeviceMobileAppConfigurationDeviceSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41e11-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="41e11-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="41e11-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41e11-105">MDM モバイル アプリ構成のデバイス状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="41e11-105">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="41e11-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="41e11-106">Methods</span></span>
|<span data-ttu-id="41e11-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="41e11-107">Method</span></span>|<span data-ttu-id="41e11-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="41e11-108">Return Type</span></span>|<span data-ttu-id="41e11-109">説明</span><span class="sxs-lookup"><span data-stu-id="41e11-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="41e11-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="41e11-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="41e11-111">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="41e11-111">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="41e11-112"> [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="41e11-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="41e11-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="41e11-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="41e11-114">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="41e11-114">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="41e11-115">[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="41e11-115">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="41e11-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41e11-116">Properties</span></span>
|<span data-ttu-id="41e11-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41e11-117">Property</span></span>|<span data-ttu-id="41e11-118">型</span><span class="sxs-lookup"><span data-stu-id="41e11-118">Type</span></span>|<span data-ttu-id="41e11-119">説明</span><span class="sxs-lookup"><span data-stu-id="41e11-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e11-120">id</span><span class="sxs-lookup"><span data-stu-id="41e11-120">id</span></span>|<span data-ttu-id="41e11-121">String</span><span class="sxs-lookup"><span data-stu-id="41e11-121">String</span></span>|<span data-ttu-id="41e11-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="41e11-122">Key of the entity.</span></span>|
|<span data-ttu-id="41e11-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="41e11-123">pendingCount</span></span>|<span data-ttu-id="41e11-124">Int32</span><span class="sxs-lookup"><span data-stu-id="41e11-124">Int32</span></span>|<span data-ttu-id="41e11-125">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="41e11-125">Number of pending devices</span></span>|
|<span data-ttu-id="41e11-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="41e11-126">notApplicableCount</span></span>|<span data-ttu-id="41e11-127">Int32</span><span class="sxs-lookup"><span data-stu-id="41e11-127">Int32</span></span>|<span data-ttu-id="41e11-128">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="41e11-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="41e11-129">successCount</span><span class="sxs-lookup"><span data-stu-id="41e11-129">successCount</span></span>|<span data-ttu-id="41e11-130">Int32</span><span class="sxs-lookup"><span data-stu-id="41e11-130">Int32</span></span>|<span data-ttu-id="41e11-131">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="41e11-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="41e11-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="41e11-132">errorCount</span></span>|<span data-ttu-id="41e11-133">Int32</span><span class="sxs-lookup"><span data-stu-id="41e11-133">Int32</span></span>|<span data-ttu-id="41e11-134">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="41e11-134">Number of error devices</span></span>|
|<span data-ttu-id="41e11-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="41e11-135">failedCount</span></span>|<span data-ttu-id="41e11-136">Int32</span><span class="sxs-lookup"><span data-stu-id="41e11-136">Int32</span></span>|<span data-ttu-id="41e11-137">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="41e11-137">Number of failed devices</span></span>|
|<span data-ttu-id="41e11-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="41e11-138">lastUpdateDateTime</span></span>|<span data-ttu-id="41e11-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41e11-139">DateTimeOffset</span></span>|<span data-ttu-id="41e11-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="41e11-140">Last update time</span></span>|
|<span data-ttu-id="41e11-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="41e11-141">configurationVersion</span></span>|<span data-ttu-id="41e11-142">Int32</span><span class="sxs-lookup"><span data-stu-id="41e11-142">Int32</span></span>|<span data-ttu-id="41e11-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="41e11-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="41e11-144">関係</span><span class="sxs-lookup"><span data-stu-id="41e11-144">Relationships</span></span>
<span data-ttu-id="41e11-145">なし</span><span class="sxs-lookup"><span data-stu-id="41e11-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41e11-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41e11-146">JSON Representation</span></span>
<span data-ttu-id="41e11-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41e11-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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



