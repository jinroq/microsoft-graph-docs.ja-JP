---
title: mobileAppInstallStatus リソースの種類
description: デバイス用のモバイルアプリのインストール状態のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2531bebd9a7cca2880ac0373b07d64ddba6cae4f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949928"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="29fab-103">mobileAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29fab-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="29fab-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29fab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29fab-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29fab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29fab-106">デバイス用のモバイルアプリのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="29fab-106">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="29fab-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="29fab-107">Methods</span></span>
|<span data-ttu-id="29fab-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="29fab-108">Method</span></span>|<span data-ttu-id="29fab-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="29fab-109">Return Type</span></span>|<span data-ttu-id="29fab-110">説明</span><span class="sxs-lookup"><span data-stu-id="29fab-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29fab-111">リスト mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="29fab-111">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="29fab-112">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29fab-112">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="29fab-113">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="29fab-113">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="29fab-114">MobileAppInstallStatus を取得する</span><span class="sxs-lookup"><span data-stu-id="29fab-114">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="29fab-115">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="29fab-115">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="29fab-116">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="29fab-116">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="29fab-117">MobileAppInstallStatus を作成する</span><span class="sxs-lookup"><span data-stu-id="29fab-117">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="29fab-118">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="29fab-118">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="29fab-119">新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="29fab-119">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="29fab-120">MobileAppInstallStatus の削除</span><span class="sxs-lookup"><span data-stu-id="29fab-120">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="29fab-121">None</span><span class="sxs-lookup"><span data-stu-id="29fab-121">None</span></span>|<span data-ttu-id="29fab-122">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="29fab-122">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="29fab-123">MobileAppInstallStatus の更新</span><span class="sxs-lookup"><span data-stu-id="29fab-123">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="29fab-124">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="29fab-124">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="29fab-125">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="29fab-125">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29fab-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29fab-126">Properties</span></span>
|<span data-ttu-id="29fab-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29fab-127">Property</span></span>|<span data-ttu-id="29fab-128">種類</span><span class="sxs-lookup"><span data-stu-id="29fab-128">Type</span></span>|<span data-ttu-id="29fab-129">説明</span><span class="sxs-lookup"><span data-stu-id="29fab-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29fab-130">id</span><span class="sxs-lookup"><span data-stu-id="29fab-130">id</span></span>|<span data-ttu-id="29fab-131">文字列</span><span class="sxs-lookup"><span data-stu-id="29fab-131">String</span></span>|<span data-ttu-id="29fab-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="29fab-132">Key of the entity.</span></span>|
|<span data-ttu-id="29fab-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="29fab-133">deviceName</span></span>|<span data-ttu-id="29fab-134">String</span><span class="sxs-lookup"><span data-stu-id="29fab-134">String</span></span>|<span data-ttu-id="29fab-135">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="29fab-135">Device name</span></span>|
|<span data-ttu-id="29fab-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="29fab-136">deviceId</span></span>|<span data-ttu-id="29fab-137">String</span><span class="sxs-lookup"><span data-stu-id="29fab-137">String</span></span>|<span data-ttu-id="29fab-138">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="29fab-138">Device ID</span></span>|
|<span data-ttu-id="29fab-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="29fab-139">lastSyncDateTime</span></span>|<span data-ttu-id="29fab-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29fab-140">DateTimeOffset</span></span>|<span data-ttu-id="29fab-141">最終同期日時</span><span class="sxs-lookup"><span data-stu-id="29fab-141">Last sync date time</span></span>|
|<span data-ttu-id="29fab-142">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="29fab-142">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="29fab-143">Resultappstate</span><span class="sxs-lookup"><span data-stu-id="29fab-143">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="29fab-144">アプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="29fab-144">The install state of the app.</span></span> <span data-ttu-id="29fab-145">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="29fab-145">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="29fab-146">installState</span><span class="sxs-lookup"><span data-stu-id="29fab-146">installState</span></span>|[<span data-ttu-id="29fab-147">Resultappstate</span><span class="sxs-lookup"><span data-stu-id="29fab-147">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="29fab-148">アプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="29fab-148">The install state of the app.</span></span> <span data-ttu-id="29fab-149">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="29fab-149">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="29fab-150">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="29fab-150">installStateDetail</span></span>|[<span data-ttu-id="29fab-151">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="29fab-151">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="29fab-152">アプリのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="29fab-152">The install state detail of the app.</span></span> <span data-ttu-id="29fab-153">可能な値: `noAdditionalDetails`、 `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`、、、、、、、、、、、、 `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="29fab-153">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="29fab-154">errorCode</span><span class="sxs-lookup"><span data-stu-id="29fab-154">errorCode</span></span>|<span data-ttu-id="29fab-155">Int32</span><span class="sxs-lookup"><span data-stu-id="29fab-155">Int32</span></span>|<span data-ttu-id="29fab-156">インストールまたはアンインストールの失敗のエラーコード。</span><span class="sxs-lookup"><span data-stu-id="29fab-156">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="29fab-157">osVersion</span><span class="sxs-lookup"><span data-stu-id="29fab-157">osVersion</span></span>|<span data-ttu-id="29fab-158">String</span><span class="sxs-lookup"><span data-stu-id="29fab-158">String</span></span>|<span data-ttu-id="29fab-159">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="29fab-159">OS Version</span></span>|
|<span data-ttu-id="29fab-160">osDescription</span><span class="sxs-lookup"><span data-stu-id="29fab-160">osDescription</span></span>|<span data-ttu-id="29fab-161">String</span><span class="sxs-lookup"><span data-stu-id="29fab-161">String</span></span>|<span data-ttu-id="29fab-162">OS の説明</span><span class="sxs-lookup"><span data-stu-id="29fab-162">OS Description</span></span>|
|<span data-ttu-id="29fab-163">userName</span><span class="sxs-lookup"><span data-stu-id="29fab-163">userName</span></span>|<span data-ttu-id="29fab-164">String</span><span class="sxs-lookup"><span data-stu-id="29fab-164">String</span></span>|<span data-ttu-id="29fab-165">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="29fab-165">Device User Name</span></span>|
|<span data-ttu-id="29fab-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="29fab-166">userPrincipalName</span></span>|<span data-ttu-id="29fab-167">String</span><span class="sxs-lookup"><span data-stu-id="29fab-167">String</span></span>|<span data-ttu-id="29fab-168">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="29fab-168">User Principal Name</span></span>|
|<span data-ttu-id="29fab-169">displayVersion</span><span class="sxs-lookup"><span data-stu-id="29fab-169">displayVersion</span></span>|<span data-ttu-id="29fab-170">String</span><span class="sxs-lookup"><span data-stu-id="29fab-170">String</span></span>|<span data-ttu-id="29fab-171">アプリケーションの人間の読み取り可能なバージョン</span><span class="sxs-lookup"><span data-stu-id="29fab-171">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="29fab-172">関係</span><span class="sxs-lookup"><span data-stu-id="29fab-172">Relationships</span></span>
|<span data-ttu-id="29fab-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29fab-173">Relationship</span></span>|<span data-ttu-id="29fab-174">型</span><span class="sxs-lookup"><span data-stu-id="29fab-174">Type</span></span>|<span data-ttu-id="29fab-175">説明</span><span class="sxs-lookup"><span data-stu-id="29fab-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29fab-176">アプリ</span><span class="sxs-lookup"><span data-stu-id="29fab-176">app</span></span>|[<span data-ttu-id="29fab-177">mobileApp</span><span class="sxs-lookup"><span data-stu-id="29fab-177">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="29fab-178">モバイルアプリへのナビゲーションリンク。</span><span class="sxs-lookup"><span data-stu-id="29fab-178">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29fab-179">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29fab-179">JSON Representation</span></span>
<span data-ttu-id="29fab-180">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29fab-180">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```




