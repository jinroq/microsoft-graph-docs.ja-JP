---
title: restrictedAppsViolation リソースの種類
description: 各ユーザーごとのデバイスの制限されたアプリケーションの構成プロファイルの違反
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcbd7def59d17dcd6e906e1e6bef85e3a448b880
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424981"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="0d39c-103">restrictedAppsViolation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d39c-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="0d39c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d39c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d39c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d39c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d39c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d39c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d39c-107">各ユーザーごとのデバイスの制限されたアプリケーションの構成プロファイルの違反</span><span class="sxs-lookup"><span data-stu-id="0d39c-107">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="0d39c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d39c-108">Methods</span></span>
|<span data-ttu-id="0d39c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d39c-109">Method</span></span>|<span data-ttu-id="0d39c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0d39c-110">Return Type</span></span>|<span data-ttu-id="0d39c-111">説明</span><span class="sxs-lookup"><span data-stu-id="0d39c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0d39c-112">リスト restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="0d39c-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="0d39c-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d39c-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="0d39c-114">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="0d39c-115">RestrictedAppsViolation を取得します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="0d39c-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="0d39c-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="0d39c-117">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d39c-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="0d39c-118">RestrictedAppsViolation を作成します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="0d39c-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="0d39c-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="0d39c-120">新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="0d39c-121">RestrictedAppsViolation を削除します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="0d39c-122">なし</span><span class="sxs-lookup"><span data-stu-id="0d39c-122">None</span></span>|<span data-ttu-id="0d39c-123">の[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="0d39c-124">RestrictedAppsViolation を更新します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="0d39c-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="0d39c-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="0d39c-126">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d39c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d39c-127">Properties</span></span>
|<span data-ttu-id="0d39c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d39c-128">Property</span></span>|<span data-ttu-id="0d39c-129">型</span><span class="sxs-lookup"><span data-stu-id="0d39c-129">Type</span></span>|<span data-ttu-id="0d39c-130">説明</span><span class="sxs-lookup"><span data-stu-id="0d39c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d39c-131">id</span><span class="sxs-lookup"><span data-stu-id="0d39c-131">id</span></span>|<span data-ttu-id="0d39c-132">String</span><span class="sxs-lookup"><span data-stu-id="0d39c-132">String</span></span>|<span data-ttu-id="0d39c-133">オブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="0d39c-133">Unique identifier for the object.</span></span> <span data-ttu-id="0d39c-134">"Accountid"、deviceId、policyId、およびユーザー Id から構成されます。</span><span class="sxs-lookup"><span data-stu-id="0d39c-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="0d39c-135">userId</span><span class="sxs-lookup"><span data-stu-id="0d39c-135">userId</span></span>|<span data-ttu-id="0d39c-136">String</span><span class="sxs-lookup"><span data-stu-id="0d39c-136">String</span></span>|<span data-ttu-id="0d39c-137">ユーザーの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d39c-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="0d39c-138">userName</span><span class="sxs-lookup"><span data-stu-id="0d39c-138">userName</span></span>|<span data-ttu-id="0d39c-139">String</span><span class="sxs-lookup"><span data-stu-id="0d39c-139">String</span></span>|<span data-ttu-id="0d39c-140">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="0d39c-140">User name</span></span>|
|<span data-ttu-id="0d39c-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0d39c-141">managedDeviceId</span></span>|<span data-ttu-id="0d39c-142">String</span><span class="sxs-lookup"><span data-stu-id="0d39c-142">String</span></span>|<span data-ttu-id="0d39c-143">管理対象デバイスの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d39c-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="0d39c-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="0d39c-144">deviceName</span></span>|<span data-ttu-id="0d39c-145">String</span><span class="sxs-lookup"><span data-stu-id="0d39c-145">String</span></span>|<span data-ttu-id="0d39c-146">デバイス名</span><span class="sxs-lookup"><span data-stu-id="0d39c-146">Device name</span></span>|
|<span data-ttu-id="0d39c-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="0d39c-147">deviceConfigurationId</span></span>|<span data-ttu-id="0d39c-148">String</span><span class="sxs-lookup"><span data-stu-id="0d39c-148">String</span></span>|<span data-ttu-id="0d39c-149">デバイス構成プロファイルの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d39c-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="0d39c-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="0d39c-150">deviceConfigurationName</span></span>|<span data-ttu-id="0d39c-151">String</span><span class="sxs-lookup"><span data-stu-id="0d39c-151">String</span></span>|<span data-ttu-id="0d39c-152">デバイス構成のプロファイル名</span><span class="sxs-lookup"><span data-stu-id="0d39c-152">Device configuration profile name</span></span>|
|<span data-ttu-id="0d39c-153">platformType</span><span class="sxs-lookup"><span data-stu-id="0d39c-153">platformType</span></span>|[<span data-ttu-id="0d39c-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="0d39c-154">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="0d39c-155">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="0d39c-155">Platform type.</span></span> <span data-ttu-id="0d39c-156">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="0d39c-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="0d39c-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="0d39c-157">restrictedAppsState</span></span>|[<span data-ttu-id="0d39c-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="0d39c-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="0d39c-159">アプリケーションの状態を制限します。</span><span class="sxs-lookup"><span data-stu-id="0d39c-159">Restricted apps state.</span></span> <span data-ttu-id="0d39c-160">使用可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="0d39c-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="0d39c-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="0d39c-161">restrictedApps</span></span>|<span data-ttu-id="0d39c-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d39c-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="0d39c-163">違反した制限されたアプリケーションの一覧</span><span class="sxs-lookup"><span data-stu-id="0d39c-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d39c-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0d39c-164">Relationships</span></span>
<span data-ttu-id="0d39c-165">なし</span><span class="sxs-lookup"><span data-stu-id="0d39c-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d39c-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d39c-166">JSON Representation</span></span>
<span data-ttu-id="0d39c-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0d39c-167">Here is a JSON representation of the resource.</span></span>
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




