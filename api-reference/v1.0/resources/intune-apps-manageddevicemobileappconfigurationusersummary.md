---
title: managedDeviceMobileAppConfigurationUserSummary リソースの種類
description: MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 385e9ac51b10d97e425cf19acb10007402eeeeb4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934892"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="09062-103">managedDeviceMobileAppConfigurationUserSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09062-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="09062-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="09062-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09062-105">MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="09062-105">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="09062-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="09062-106">Methods</span></span>
|<span data-ttu-id="09062-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="09062-107">Method</span></span>|<span data-ttu-id="09062-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="09062-108">Return Type</span></span>|<span data-ttu-id="09062-109">説明</span><span class="sxs-lookup"><span data-stu-id="09062-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="09062-110">managedDeviceMobileAppConfigurationUserSummary の取得</span><span class="sxs-lookup"><span data-stu-id="09062-110">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="09062-111">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="09062-111">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="09062-112">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="09062-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="09062-113">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="09062-113">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="09062-114">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="09062-114">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="09062-115">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="09062-115">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09062-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09062-116">Properties</span></span>
|<span data-ttu-id="09062-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09062-117">Property</span></span>|<span data-ttu-id="09062-118">種類</span><span class="sxs-lookup"><span data-stu-id="09062-118">Type</span></span>|<span data-ttu-id="09062-119">説明</span><span class="sxs-lookup"><span data-stu-id="09062-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09062-120">ID</span><span class="sxs-lookup"><span data-stu-id="09062-120">id</span></span>|<span data-ttu-id="09062-121">String</span><span class="sxs-lookup"><span data-stu-id="09062-121">String</span></span>|<span data-ttu-id="09062-122">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="09062-122">Key of the entity.</span></span>|
|<span data-ttu-id="09062-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="09062-123">pendingCount</span></span>|<span data-ttu-id="09062-124">Int32</span><span class="sxs-lookup"><span data-stu-id="09062-124">Int32</span></span>|<span data-ttu-id="09062-125">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="09062-125">Number of pending Users</span></span>|
|<span data-ttu-id="09062-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="09062-126">notApplicableCount</span></span>|<span data-ttu-id="09062-127">Int32</span><span class="sxs-lookup"><span data-stu-id="09062-127">Int32</span></span>|<span data-ttu-id="09062-128">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="09062-128">Number of not applicable users</span></span>|
|<span data-ttu-id="09062-129">successCount</span><span class="sxs-lookup"><span data-stu-id="09062-129">successCount</span></span>|<span data-ttu-id="09062-130">Int32</span><span class="sxs-lookup"><span data-stu-id="09062-130">Int32</span></span>|<span data-ttu-id="09062-131">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="09062-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="09062-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="09062-132">errorCount</span></span>|<span data-ttu-id="09062-133">Int32</span><span class="sxs-lookup"><span data-stu-id="09062-133">Int32</span></span>|<span data-ttu-id="09062-134">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="09062-134">Number of error Users</span></span>|
|<span data-ttu-id="09062-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="09062-135">failedCount</span></span>|<span data-ttu-id="09062-136">Int32</span><span class="sxs-lookup"><span data-stu-id="09062-136">Int32</span></span>|<span data-ttu-id="09062-137">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="09062-137">Number of failed Users</span></span>|
|<span data-ttu-id="09062-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="09062-138">lastUpdateDateTime</span></span>|<span data-ttu-id="09062-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09062-139">DateTimeOffset</span></span>|<span data-ttu-id="09062-140">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="09062-140">Last update time</span></span>|
|<span data-ttu-id="09062-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="09062-141">configurationVersion</span></span>|<span data-ttu-id="09062-142">Int32</span><span class="sxs-lookup"><span data-stu-id="09062-142">Int32</span></span>|<span data-ttu-id="09062-143">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="09062-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="09062-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09062-144">Relationships</span></span>
<span data-ttu-id="09062-145">なし</span><span class="sxs-lookup"><span data-stu-id="09062-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09062-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09062-146">JSON Representation</span></span>
<span data-ttu-id="09062-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09062-147">Here is a JSON representation of the resource.</span></span>
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



