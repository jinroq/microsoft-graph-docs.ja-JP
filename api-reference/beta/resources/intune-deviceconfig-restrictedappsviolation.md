---
title: restrictedAppsViolation リソースの種類
description: ユーザーごとのデバイスごとの制限付きアプリ構成プロファイルの違反
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8764d3d84ba0706f3769ef019def43cb080660d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139915"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="9d582-103">restrictedAppsViolation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9d582-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="9d582-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d582-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d582-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d582-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d582-106">ユーザーごとのデバイスごとの制限付きアプリ構成プロファイルの違反</span><span class="sxs-lookup"><span data-stu-id="9d582-106">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="9d582-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9d582-107">Methods</span></span>
|<span data-ttu-id="9d582-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9d582-108">Method</span></span>|<span data-ttu-id="9d582-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9d582-109">Return Type</span></span>|<span data-ttu-id="9d582-110">説明</span><span class="sxs-lookup"><span data-stu-id="9d582-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9d582-111">リスト restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="9d582-111">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="9d582-112">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9d582-112">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="9d582-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9d582-113">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="9d582-114">restrictedAppsViolation を取得する</span><span class="sxs-lookup"><span data-stu-id="9d582-114">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="9d582-115">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="9d582-115">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="9d582-116">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9d582-116">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="9d582-117">restrictedAppsViolation を作成する</span><span class="sxs-lookup"><span data-stu-id="9d582-117">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="9d582-118">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="9d582-118">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="9d582-119">新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9d582-119">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="9d582-120">restrictedAppsViolation の削除</span><span class="sxs-lookup"><span data-stu-id="9d582-120">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="9d582-121">なし</span><span class="sxs-lookup"><span data-stu-id="9d582-121">None</span></span>|<span data-ttu-id="9d582-122">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="9d582-122">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="9d582-123">restrictedAppsViolation の更新</span><span class="sxs-lookup"><span data-stu-id="9d582-123">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="9d582-124">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="9d582-124">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="9d582-125">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9d582-125">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9d582-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d582-126">Properties</span></span>
|<span data-ttu-id="9d582-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d582-127">Property</span></span>|<span data-ttu-id="9d582-128">型</span><span class="sxs-lookup"><span data-stu-id="9d582-128">Type</span></span>|<span data-ttu-id="9d582-129">説明</span><span class="sxs-lookup"><span data-stu-id="9d582-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d582-130">id</span><span class="sxs-lookup"><span data-stu-id="9d582-130">id</span></span>|<span data-ttu-id="9d582-131">文字列</span><span class="sxs-lookup"><span data-stu-id="9d582-131">String</span></span>|<span data-ttu-id="9d582-132">オブジェクトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="9d582-132">Unique identifier for the object.</span></span> <span data-ttu-id="9d582-133">accountId、deviceId、policyid、および userId から構成されます。</span><span class="sxs-lookup"><span data-stu-id="9d582-133">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="9d582-134">userId</span><span class="sxs-lookup"><span data-stu-id="9d582-134">userId</span></span>|<span data-ttu-id="9d582-135">String</span><span class="sxs-lookup"><span data-stu-id="9d582-135">String</span></span>|<span data-ttu-id="9d582-136">ユーザーの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="9d582-136">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9d582-137">userName</span><span class="sxs-lookup"><span data-stu-id="9d582-137">userName</span></span>|<span data-ttu-id="9d582-138">String</span><span class="sxs-lookup"><span data-stu-id="9d582-138">String</span></span>|<span data-ttu-id="9d582-139">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="9d582-139">User name</span></span>|
|<span data-ttu-id="9d582-140">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="9d582-140">managedDeviceId</span></span>|<span data-ttu-id="9d582-141">String</span><span class="sxs-lookup"><span data-stu-id="9d582-141">String</span></span>|<span data-ttu-id="9d582-142">管理デバイスの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="9d582-142">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9d582-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="9d582-143">deviceName</span></span>|<span data-ttu-id="9d582-144">String</span><span class="sxs-lookup"><span data-stu-id="9d582-144">String</span></span>|<span data-ttu-id="9d582-145">デバイス名</span><span class="sxs-lookup"><span data-stu-id="9d582-145">Device name</span></span>|
|<span data-ttu-id="9d582-146">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="9d582-146">deviceConfigurationId</span></span>|<span data-ttu-id="9d582-147">String</span><span class="sxs-lookup"><span data-stu-id="9d582-147">String</span></span>|<span data-ttu-id="9d582-148">デバイス構成プロファイルの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="9d582-148">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9d582-149">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="9d582-149">deviceConfigurationName</span></span>|<span data-ttu-id="9d582-150">String</span><span class="sxs-lookup"><span data-stu-id="9d582-150">String</span></span>|<span data-ttu-id="9d582-151">デバイス構成プロファイル名</span><span class="sxs-lookup"><span data-stu-id="9d582-151">Device configuration profile name</span></span>|
|<span data-ttu-id="9d582-152">platformType</span><span class="sxs-lookup"><span data-stu-id="9d582-152">platformType</span></span>|[<span data-ttu-id="9d582-153">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="9d582-153">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="9d582-154">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="9d582-154">Platform type.</span></span> <span data-ttu-id="9d582-155">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="9d582-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="9d582-156">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="9d582-156">restrictedAppsState</span></span>|[<span data-ttu-id="9d582-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="9d582-157">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="9d582-158">制限付きアプリの状態。</span><span class="sxs-lookup"><span data-stu-id="9d582-158">Restricted apps state.</span></span> <span data-ttu-id="9d582-159">使用可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="9d582-159">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="9d582-160">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="9d582-160">restrictedApps</span></span>|<span data-ttu-id="9d582-161">[manageddevicereportedapp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9d582-161">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="9d582-162">違反した制限付きアプリの一覧</span><span class="sxs-lookup"><span data-stu-id="9d582-162">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d582-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9d582-163">Relationships</span></span>
<span data-ttu-id="9d582-164">なし</span><span class="sxs-lookup"><span data-stu-id="9d582-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d582-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d582-165">JSON Representation</span></span>
<span data-ttu-id="9d582-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9d582-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```




