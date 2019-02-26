---
title: managedDeviceMobileAppConfigurationUserSummary リソースの種類
description: MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96ec2f44864e29f374ab9ccf3f63a65a91692087
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253443"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="5a969-103">managedDeviceMobileAppConfigurationUserSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a969-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="5a969-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a969-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a969-105">MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a969-105">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="5a969-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a969-106">Methods</span></span>
|<span data-ttu-id="5a969-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a969-107">Method</span></span>|<span data-ttu-id="5a969-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a969-108">Return Type</span></span>|<span data-ttu-id="5a969-109">説明</span><span class="sxs-lookup"><span data-stu-id="5a969-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a969-110">managedDeviceMobileAppConfigurationUserSummary の取得</span><span class="sxs-lookup"><span data-stu-id="5a969-110">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="5a969-111">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="5a969-111">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="5a969-112">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5a969-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="5a969-113">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="5a969-113">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="5a969-114">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="5a969-114">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="5a969-115">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a969-115">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a969-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a969-116">Properties</span></span>
|<span data-ttu-id="5a969-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a969-117">Property</span></span>|<span data-ttu-id="5a969-118">型</span><span class="sxs-lookup"><span data-stu-id="5a969-118">Type</span></span>|<span data-ttu-id="5a969-119">説明</span><span class="sxs-lookup"><span data-stu-id="5a969-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a969-120">id</span><span class="sxs-lookup"><span data-stu-id="5a969-120">id</span></span>|<span data-ttu-id="5a969-121">String</span><span class="sxs-lookup"><span data-stu-id="5a969-121">String</span></span>|<span data-ttu-id="5a969-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5a969-122">Key of the entity.</span></span>|
|<span data-ttu-id="5a969-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="5a969-123">pendingCount</span></span>|<span data-ttu-id="5a969-124">Int32</span><span class="sxs-lookup"><span data-stu-id="5a969-124">Int32</span></span>|<span data-ttu-id="5a969-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="5a969-125">Number of pending Users</span></span>|
|<span data-ttu-id="5a969-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="5a969-126">notApplicableCount</span></span>|<span data-ttu-id="5a969-127">Int32</span><span class="sxs-lookup"><span data-stu-id="5a969-127">Int32</span></span>|<span data-ttu-id="5a969-128">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="5a969-128">Number of not applicable users</span></span>|
|<span data-ttu-id="5a969-129">successCount</span><span class="sxs-lookup"><span data-stu-id="5a969-129">successCount</span></span>|<span data-ttu-id="5a969-130">Int32</span><span class="sxs-lookup"><span data-stu-id="5a969-130">Int32</span></span>|<span data-ttu-id="5a969-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="5a969-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="5a969-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="5a969-132">errorCount</span></span>|<span data-ttu-id="5a969-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5a969-133">Int32</span></span>|<span data-ttu-id="5a969-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="5a969-134">Number of error Users</span></span>|
|<span data-ttu-id="5a969-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="5a969-135">failedCount</span></span>|<span data-ttu-id="5a969-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5a969-136">Int32</span></span>|<span data-ttu-id="5a969-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="5a969-137">Number of failed Users</span></span>|
|<span data-ttu-id="5a969-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="5a969-138">lastUpdateDateTime</span></span>|<span data-ttu-id="5a969-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a969-139">DateTimeOffset</span></span>|<span data-ttu-id="5a969-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="5a969-140">Last update time</span></span>|
|<span data-ttu-id="5a969-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="5a969-141">configurationVersion</span></span>|<span data-ttu-id="5a969-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5a969-142">Int32</span></span>|<span data-ttu-id="5a969-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="5a969-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a969-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a969-144">Relationships</span></span>
<span data-ttu-id="5a969-145">なし</span><span class="sxs-lookup"><span data-stu-id="5a969-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a969-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a969-146">JSON Representation</span></span>
<span data-ttu-id="5a969-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a969-147">Here is a JSON representation of the resource.</span></span>
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
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



