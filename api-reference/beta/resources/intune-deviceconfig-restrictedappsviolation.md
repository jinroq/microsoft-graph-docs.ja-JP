---
title: restrictedAppsViolation リソースの種類
description: ユーザーごとのデバイスごとの制限付きアプリ構成プロファイルの違反
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27477d0f12b130975abe42f8b994282e5de5bbcb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986698"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="dca34-103">restrictedAppsViolation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dca34-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="dca34-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dca34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dca34-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dca34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dca34-106">ユーザーごとのデバイスごとの制限付きアプリ構成プロファイルの違反</span><span class="sxs-lookup"><span data-stu-id="dca34-106">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="dca34-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dca34-107">Methods</span></span>
|<span data-ttu-id="dca34-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dca34-108">Method</span></span>|<span data-ttu-id="dca34-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dca34-109">Return Type</span></span>|<span data-ttu-id="dca34-110">説明</span><span class="sxs-lookup"><span data-stu-id="dca34-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dca34-111">リスト restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="dca34-111">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="dca34-112">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dca34-112">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="dca34-113">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dca34-113">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="dca34-114">RestrictedAppsViolation を取得する</span><span class="sxs-lookup"><span data-stu-id="dca34-114">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="dca34-115">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="dca34-115">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="dca34-116">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dca34-116">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="dca34-117">RestrictedAppsViolation を作成する</span><span class="sxs-lookup"><span data-stu-id="dca34-117">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="dca34-118">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="dca34-118">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="dca34-119">新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dca34-119">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="dca34-120">RestrictedAppsViolation の削除</span><span class="sxs-lookup"><span data-stu-id="dca34-120">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="dca34-121">None</span><span class="sxs-lookup"><span data-stu-id="dca34-121">None</span></span>|<span data-ttu-id="dca34-122">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="dca34-122">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="dca34-123">RestrictedAppsViolation の更新</span><span class="sxs-lookup"><span data-stu-id="dca34-123">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="dca34-124">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="dca34-124">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="dca34-125">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dca34-125">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dca34-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dca34-126">Properties</span></span>
|<span data-ttu-id="dca34-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dca34-127">Property</span></span>|<span data-ttu-id="dca34-128">型</span><span class="sxs-lookup"><span data-stu-id="dca34-128">Type</span></span>|<span data-ttu-id="dca34-129">説明</span><span class="sxs-lookup"><span data-stu-id="dca34-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca34-130">id</span><span class="sxs-lookup"><span data-stu-id="dca34-130">id</span></span>|<span data-ttu-id="dca34-131">文字列</span><span class="sxs-lookup"><span data-stu-id="dca34-131">String</span></span>|<span data-ttu-id="dca34-132">オブジェクトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="dca34-132">Unique identifier for the object.</span></span> <span data-ttu-id="dca34-133">AccountId、deviceId、policyId、および userId から構成されます。</span><span class="sxs-lookup"><span data-stu-id="dca34-133">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="dca34-134">userId</span><span class="sxs-lookup"><span data-stu-id="dca34-134">userId</span></span>|<span data-ttu-id="dca34-135">String</span><span class="sxs-lookup"><span data-stu-id="dca34-135">String</span></span>|<span data-ttu-id="dca34-136">ユーザーの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="dca34-136">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="dca34-137">userName</span><span class="sxs-lookup"><span data-stu-id="dca34-137">userName</span></span>|<span data-ttu-id="dca34-138">String</span><span class="sxs-lookup"><span data-stu-id="dca34-138">String</span></span>|<span data-ttu-id="dca34-139">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="dca34-139">User name</span></span>|
|<span data-ttu-id="dca34-140">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="dca34-140">managedDeviceId</span></span>|<span data-ttu-id="dca34-141">String</span><span class="sxs-lookup"><span data-stu-id="dca34-141">String</span></span>|<span data-ttu-id="dca34-142">管理デバイスの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="dca34-142">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="dca34-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="dca34-143">deviceName</span></span>|<span data-ttu-id="dca34-144">String</span><span class="sxs-lookup"><span data-stu-id="dca34-144">String</span></span>|<span data-ttu-id="dca34-145">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="dca34-145">Device name</span></span>|
|<span data-ttu-id="dca34-146">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="dca34-146">deviceConfigurationId</span></span>|<span data-ttu-id="dca34-147">String</span><span class="sxs-lookup"><span data-stu-id="dca34-147">String</span></span>|<span data-ttu-id="dca34-148">デバイス構成プロファイルの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="dca34-148">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="dca34-149">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="dca34-149">deviceConfigurationName</span></span>|<span data-ttu-id="dca34-150">String</span><span class="sxs-lookup"><span data-stu-id="dca34-150">String</span></span>|<span data-ttu-id="dca34-151">デバイス構成プロファイル名</span><span class="sxs-lookup"><span data-stu-id="dca34-151">Device configuration profile name</span></span>|
|<span data-ttu-id="dca34-152">platformType</span><span class="sxs-lookup"><span data-stu-id="dca34-152">platformType</span></span>|[<span data-ttu-id="dca34-153">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="dca34-153">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="dca34-154">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="dca34-154">Platform type.</span></span> <span data-ttu-id="dca34-155">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="dca34-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="dca34-156">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="dca34-156">restrictedAppsState</span></span>|[<span data-ttu-id="dca34-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="dca34-157">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="dca34-158">制限付きアプリの状態。</span><span class="sxs-lookup"><span data-stu-id="dca34-158">Restricted apps state.</span></span> <span data-ttu-id="dca34-159">可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="dca34-159">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="dca34-160">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="dca34-160">restrictedApps</span></span>|<span data-ttu-id="dca34-161">[Manageddevicereportedapp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dca34-161">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="dca34-162">違反した制限付きアプリの一覧</span><span class="sxs-lookup"><span data-stu-id="dca34-162">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="dca34-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dca34-163">Relationships</span></span>
<span data-ttu-id="dca34-164">なし</span><span class="sxs-lookup"><span data-stu-id="dca34-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dca34-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dca34-165">JSON Representation</span></span>
<span data-ttu-id="dca34-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dca34-166">Here is a JSON representation of the resource.</span></span>
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





