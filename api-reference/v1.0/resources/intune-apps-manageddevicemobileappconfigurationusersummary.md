---
title: managedDeviceMobileAppConfigurationUserSummary リソースの種類
description: MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96ec2f44864e29f374ab9ccf3f63a65a91692087
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564023"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="fd5ea-103">managedDeviceMobileAppConfigurationUserSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd5ea-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="fd5ea-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd5ea-105">MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-105">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="fd5ea-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd5ea-106">Methods</span></span>
|<span data-ttu-id="fd5ea-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd5ea-107">Method</span></span>|<span data-ttu-id="fd5ea-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fd5ea-108">Return Type</span></span>|<span data-ttu-id="fd5ea-109">説明</span><span class="sxs-lookup"><span data-stu-id="fd5ea-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fd5ea-110">managedDeviceMobileAppConfigurationUserSummary の取得</span><span class="sxs-lookup"><span data-stu-id="fd5ea-110">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="fd5ea-111">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="fd5ea-111">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="fd5ea-112">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="fd5ea-113">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="fd5ea-113">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="fd5ea-114">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="fd5ea-114">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="fd5ea-115">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-115">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd5ea-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd5ea-116">Properties</span></span>
|<span data-ttu-id="fd5ea-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd5ea-117">Property</span></span>|<span data-ttu-id="fd5ea-118">型</span><span class="sxs-lookup"><span data-stu-id="fd5ea-118">Type</span></span>|<span data-ttu-id="fd5ea-119">説明</span><span class="sxs-lookup"><span data-stu-id="fd5ea-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd5ea-120">id</span><span class="sxs-lookup"><span data-stu-id="fd5ea-120">id</span></span>|<span data-ttu-id="fd5ea-121">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-121">String</span></span>|<span data-ttu-id="fd5ea-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-122">Key of the entity.</span></span>|
|<span data-ttu-id="fd5ea-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="fd5ea-123">pendingCount</span></span>|<span data-ttu-id="fd5ea-124">Int32</span><span class="sxs-lookup"><span data-stu-id="fd5ea-124">Int32</span></span>|<span data-ttu-id="fd5ea-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="fd5ea-125">Number of pending Users</span></span>|
|<span data-ttu-id="fd5ea-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="fd5ea-126">notApplicableCount</span></span>|<span data-ttu-id="fd5ea-127">Int32</span><span class="sxs-lookup"><span data-stu-id="fd5ea-127">Int32</span></span>|<span data-ttu-id="fd5ea-128">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="fd5ea-128">Number of not applicable users</span></span>|
|<span data-ttu-id="fd5ea-129">successCount</span><span class="sxs-lookup"><span data-stu-id="fd5ea-129">successCount</span></span>|<span data-ttu-id="fd5ea-130">Int32</span><span class="sxs-lookup"><span data-stu-id="fd5ea-130">Int32</span></span>|<span data-ttu-id="fd5ea-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="fd5ea-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="fd5ea-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="fd5ea-132">errorCount</span></span>|<span data-ttu-id="fd5ea-133">Int32</span><span class="sxs-lookup"><span data-stu-id="fd5ea-133">Int32</span></span>|<span data-ttu-id="fd5ea-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="fd5ea-134">Number of error Users</span></span>|
|<span data-ttu-id="fd5ea-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="fd5ea-135">failedCount</span></span>|<span data-ttu-id="fd5ea-136">Int32</span><span class="sxs-lookup"><span data-stu-id="fd5ea-136">Int32</span></span>|<span data-ttu-id="fd5ea-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="fd5ea-137">Number of failed Users</span></span>|
|<span data-ttu-id="fd5ea-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="fd5ea-138">lastUpdateDateTime</span></span>|<span data-ttu-id="fd5ea-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd5ea-139">DateTimeOffset</span></span>|<span data-ttu-id="fd5ea-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="fd5ea-140">Last update time</span></span>|
|<span data-ttu-id="fd5ea-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="fd5ea-141">configurationVersion</span></span>|<span data-ttu-id="fd5ea-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fd5ea-142">Int32</span></span>|<span data-ttu-id="fd5ea-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="fd5ea-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd5ea-144">関係</span><span class="sxs-lookup"><span data-stu-id="fd5ea-144">Relationships</span></span>
<span data-ttu-id="fd5ea-145">なし</span><span class="sxs-lookup"><span data-stu-id="fd5ea-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd5ea-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd5ea-146">JSON Representation</span></span>
<span data-ttu-id="fd5ea-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-147">Here is a JSON representation of the resource.</span></span>
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



