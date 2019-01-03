---
title: restrictedAppsViolation リソースの種類
description: 各ユーザーごとのデバイスの制限されたアプリケーションの構成プロファイルの違反
author: tfitzmac
ms.openlocfilehash: cb614bc56f27281198fcecb73bae2b7beddfa266
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304936"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="51418-103">restrictedAppsViolation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51418-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="51418-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51418-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51418-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51418-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51418-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51418-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51418-107">各ユーザーごとのデバイスの制限されたアプリケーションの構成プロファイルの違反</span><span class="sxs-lookup"><span data-stu-id="51418-107">Violation of restricted apps configuration profile per device per user</span></span>
## <a name="methods"></a><span data-ttu-id="51418-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="51418-108">Methods</span></span>
|<span data-ttu-id="51418-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="51418-109">Method</span></span>|<span data-ttu-id="51418-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="51418-110">Return Type</span></span>|<span data-ttu-id="51418-111">説明</span><span class="sxs-lookup"><span data-stu-id="51418-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51418-112">リスト restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="51418-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="51418-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="51418-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="51418-114">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="51418-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="51418-115">RestrictedAppsViolation を取得します。</span><span class="sxs-lookup"><span data-stu-id="51418-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="51418-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="51418-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="51418-117">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51418-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="51418-118">RestrictedAppsViolation を作成します。</span><span class="sxs-lookup"><span data-stu-id="51418-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="51418-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="51418-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="51418-120">新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="51418-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="51418-121">RestrictedAppsViolation を削除します。</span><span class="sxs-lookup"><span data-stu-id="51418-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="51418-122">なし</span><span class="sxs-lookup"><span data-stu-id="51418-122">None</span></span>|<span data-ttu-id="51418-123">の[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="51418-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="51418-124">RestrictedAppsViolation を更新します。</span><span class="sxs-lookup"><span data-stu-id="51418-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="51418-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="51418-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="51418-126">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="51418-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="51418-127">Properties</span><span class="sxs-lookup"><span data-stu-id="51418-127">Properties</span></span>
|<span data-ttu-id="51418-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51418-128">Property</span></span>|<span data-ttu-id="51418-129">種類</span><span class="sxs-lookup"><span data-stu-id="51418-129">Type</span></span>|<span data-ttu-id="51418-130">説明</span><span class="sxs-lookup"><span data-stu-id="51418-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51418-131">ID</span><span class="sxs-lookup"><span data-stu-id="51418-131">id</span></span>|<span data-ttu-id="51418-132">String</span><span class="sxs-lookup"><span data-stu-id="51418-132">String</span></span>|<span data-ttu-id="51418-133">オブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="51418-133">Unique identifier for the object.</span></span> <span data-ttu-id="51418-134">"Accountid"、deviceId、policyId、およびユーザー Id から構成されます。</span><span class="sxs-lookup"><span data-stu-id="51418-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="51418-135">userId</span><span class="sxs-lookup"><span data-stu-id="51418-135">userId</span></span>|<span data-ttu-id="51418-136">String</span><span class="sxs-lookup"><span data-stu-id="51418-136">String</span></span>|<span data-ttu-id="51418-137">ユーザーの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="51418-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="51418-138">userName</span><span class="sxs-lookup"><span data-stu-id="51418-138">userName</span></span>|<span data-ttu-id="51418-139">String</span><span class="sxs-lookup"><span data-stu-id="51418-139">String</span></span>|<span data-ttu-id="51418-140">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="51418-140">User name</span></span>|
|<span data-ttu-id="51418-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="51418-141">managedDeviceId</span></span>|<span data-ttu-id="51418-142">String</span><span class="sxs-lookup"><span data-stu-id="51418-142">String</span></span>|<span data-ttu-id="51418-143">管理対象デバイスの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="51418-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="51418-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="51418-144">deviceName</span></span>|<span data-ttu-id="51418-145">String</span><span class="sxs-lookup"><span data-stu-id="51418-145">String</span></span>|<span data-ttu-id="51418-146">デバイス名</span><span class="sxs-lookup"><span data-stu-id="51418-146">Device name</span></span>|
|<span data-ttu-id="51418-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="51418-147">deviceConfigurationId</span></span>|<span data-ttu-id="51418-148">String</span><span class="sxs-lookup"><span data-stu-id="51418-148">String</span></span>|<span data-ttu-id="51418-149">デバイス構成プロファイルの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="51418-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="51418-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="51418-150">deviceConfigurationName</span></span>|<span data-ttu-id="51418-151">String</span><span class="sxs-lookup"><span data-stu-id="51418-151">String</span></span>|<span data-ttu-id="51418-152">デバイス構成のプロファイル名</span><span class="sxs-lookup"><span data-stu-id="51418-152">Device configuration profile name</span></span>|
|<span data-ttu-id="51418-153">platformType</span><span class="sxs-lookup"><span data-stu-id="51418-153">platformType</span></span>|[<span data-ttu-id="51418-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="51418-154">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="51418-155">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="51418-155">Platform type.</span></span> <span data-ttu-id="51418-156">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="51418-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="51418-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="51418-157">restrictedAppsState</span></span>|[<span data-ttu-id="51418-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="51418-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="51418-159">アプリケーションの状態を制限します。</span><span class="sxs-lookup"><span data-stu-id="51418-159">Restricted apps state.</span></span> <span data-ttu-id="51418-160">使用可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="51418-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="51418-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="51418-161">restrictedApps</span></span>|<span data-ttu-id="51418-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="51418-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="51418-163">違反した制限されたアプリケーションの一覧</span><span class="sxs-lookup"><span data-stu-id="51418-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="51418-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51418-164">Relationships</span></span>
<span data-ttu-id="51418-165">なし</span><span class="sxs-lookup"><span data-stu-id="51418-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51418-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51418-166">JSON Representation</span></span>
<span data-ttu-id="51418-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51418-167">Here is a JSON representation of the resource.</span></span>
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




