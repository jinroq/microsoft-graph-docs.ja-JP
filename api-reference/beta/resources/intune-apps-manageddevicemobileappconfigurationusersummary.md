---
title: managedDeviceMobileAppConfigurationUserSummary リソースの種類
description: MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 05b8d23ab03e2e282666bdd18c2d06410679a822
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308261"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="bf61a-103">managedDeviceMobileAppConfigurationUserSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf61a-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="bf61a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf61a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf61a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf61a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf61a-106">MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bf61a-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="bf61a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf61a-107">Methods</span></span>
|<span data-ttu-id="bf61a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf61a-108">Method</span></span>|<span data-ttu-id="bf61a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bf61a-109">Return Type</span></span>|<span data-ttu-id="bf61a-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf61a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bf61a-111">managedDeviceMobileAppConfigurationUserSummary の取得</span><span class="sxs-lookup"><span data-stu-id="bf61a-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="bf61a-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="bf61a-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="bf61a-113">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bf61a-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="bf61a-114">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="bf61a-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="bf61a-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="bf61a-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="bf61a-116">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bf61a-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf61a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf61a-117">Properties</span></span>
|<span data-ttu-id="bf61a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf61a-118">Property</span></span>|<span data-ttu-id="bf61a-119">型</span><span class="sxs-lookup"><span data-stu-id="bf61a-119">Type</span></span>|<span data-ttu-id="bf61a-120">説明</span><span class="sxs-lookup"><span data-stu-id="bf61a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf61a-121">id</span><span class="sxs-lookup"><span data-stu-id="bf61a-121">id</span></span>|<span data-ttu-id="bf61a-122">String</span><span class="sxs-lookup"><span data-stu-id="bf61a-122">String</span></span>|<span data-ttu-id="bf61a-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bf61a-123">Key of the entity.</span></span>|
|<span data-ttu-id="bf61a-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="bf61a-124">pendingCount</span></span>|<span data-ttu-id="bf61a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bf61a-125">Int32</span></span>|<span data-ttu-id="bf61a-126">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="bf61a-126">Number of pending Users</span></span>|
|<span data-ttu-id="bf61a-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="bf61a-127">notApplicableCount</span></span>|<span data-ttu-id="bf61a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="bf61a-128">Int32</span></span>|<span data-ttu-id="bf61a-129">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="bf61a-129">Number of not applicable users</span></span>|
|<span data-ttu-id="bf61a-130">successCount</span><span class="sxs-lookup"><span data-stu-id="bf61a-130">successCount</span></span>|<span data-ttu-id="bf61a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="bf61a-131">Int32</span></span>|<span data-ttu-id="bf61a-132">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="bf61a-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="bf61a-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="bf61a-133">errorCount</span></span>|<span data-ttu-id="bf61a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="bf61a-134">Int32</span></span>|<span data-ttu-id="bf61a-135">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="bf61a-135">Number of error Users</span></span>|
|<span data-ttu-id="bf61a-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="bf61a-136">failedCount</span></span>|<span data-ttu-id="bf61a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bf61a-137">Int32</span></span>|<span data-ttu-id="bf61a-138">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="bf61a-138">Number of failed Users</span></span>|
|<span data-ttu-id="bf61a-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="bf61a-139">conflictCount</span></span>|<span data-ttu-id="bf61a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bf61a-140">Int32</span></span>|<span data-ttu-id="bf61a-141">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="bf61a-141">Number of users in conflict</span></span>|
|<span data-ttu-id="bf61a-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bf61a-142">lastUpdateDateTime</span></span>|<span data-ttu-id="bf61a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf61a-143">DateTimeOffset</span></span>|<span data-ttu-id="bf61a-144">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="bf61a-144">Last update time</span></span>|
|<span data-ttu-id="bf61a-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="bf61a-145">configurationVersion</span></span>|<span data-ttu-id="bf61a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="bf61a-146">Int32</span></span>|<span data-ttu-id="bf61a-147">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="bf61a-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf61a-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf61a-148">Relationships</span></span>
<span data-ttu-id="bf61a-149">なし</span><span class="sxs-lookup"><span data-stu-id="bf61a-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf61a-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf61a-150">JSON Representation</span></span>
<span data-ttu-id="bf61a-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf61a-151">Here is a JSON representation of the resource.</span></span>
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



