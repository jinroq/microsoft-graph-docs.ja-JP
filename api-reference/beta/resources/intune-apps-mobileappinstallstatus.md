---
title: mobileAppInstallStatus リソースの種類
description: デバイス用のモバイルアプリのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91dbe509db57153aa325ecf80c508d8ec47f69b7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162364"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="54147-103">mobileAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54147-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="54147-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54147-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54147-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54147-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54147-106">デバイス用のモバイルアプリのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54147-106">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="54147-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="54147-107">Methods</span></span>
|<span data-ttu-id="54147-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="54147-108">Method</span></span>|<span data-ttu-id="54147-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="54147-109">Return Type</span></span>|<span data-ttu-id="54147-110">説明</span><span class="sxs-lookup"><span data-stu-id="54147-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54147-111">リスト mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="54147-111">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="54147-112">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="54147-112">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="54147-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="54147-113">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="54147-114">mobileAppInstallStatus を取得する</span><span class="sxs-lookup"><span data-stu-id="54147-114">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="54147-115">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="54147-115">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="54147-116">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="54147-116">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="54147-117">mobileAppInstallStatus を作成する</span><span class="sxs-lookup"><span data-stu-id="54147-117">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="54147-118">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="54147-118">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="54147-119">新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="54147-119">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="54147-120">mobileAppInstallStatus の削除</span><span class="sxs-lookup"><span data-stu-id="54147-120">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="54147-121">なし</span><span class="sxs-lookup"><span data-stu-id="54147-121">None</span></span>|<span data-ttu-id="54147-122">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="54147-122">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="54147-123">mobileAppInstallStatus の更新</span><span class="sxs-lookup"><span data-stu-id="54147-123">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="54147-124">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="54147-124">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="54147-125">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="54147-125">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="54147-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54147-126">Properties</span></span>
|<span data-ttu-id="54147-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54147-127">Property</span></span>|<span data-ttu-id="54147-128">型</span><span class="sxs-lookup"><span data-stu-id="54147-128">Type</span></span>|<span data-ttu-id="54147-129">説明</span><span class="sxs-lookup"><span data-stu-id="54147-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54147-130">id</span><span class="sxs-lookup"><span data-stu-id="54147-130">id</span></span>|<span data-ttu-id="54147-131">String</span><span class="sxs-lookup"><span data-stu-id="54147-131">String</span></span>|<span data-ttu-id="54147-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="54147-132">Key of the entity.</span></span>|
|<span data-ttu-id="54147-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="54147-133">deviceName</span></span>|<span data-ttu-id="54147-134">String</span><span class="sxs-lookup"><span data-stu-id="54147-134">String</span></span>|<span data-ttu-id="54147-135">デバイス名</span><span class="sxs-lookup"><span data-stu-id="54147-135">Device name</span></span>|
|<span data-ttu-id="54147-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="54147-136">deviceId</span></span>|<span data-ttu-id="54147-137">String</span><span class="sxs-lookup"><span data-stu-id="54147-137">String</span></span>|<span data-ttu-id="54147-138">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="54147-138">Device ID</span></span>|
|<span data-ttu-id="54147-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="54147-139">lastSyncDateTime</span></span>|<span data-ttu-id="54147-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54147-140">DateTimeOffset</span></span>|<span data-ttu-id="54147-141">最終同期日時</span><span class="sxs-lookup"><span data-stu-id="54147-141">Last sync date time</span></span>|
|<span data-ttu-id="54147-142">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="54147-142">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="54147-143">resultappstate</span><span class="sxs-lookup"><span data-stu-id="54147-143">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="54147-144">アプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="54147-144">The install state of the app.</span></span> <span data-ttu-id="54147-145">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="54147-145">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="54147-146">installState</span><span class="sxs-lookup"><span data-stu-id="54147-146">installState</span></span>|[<span data-ttu-id="54147-147">resultappstate</span><span class="sxs-lookup"><span data-stu-id="54147-147">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="54147-148">アプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="54147-148">The install state of the app.</span></span> <span data-ttu-id="54147-149">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="54147-149">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="54147-150">installstatedetail</span><span class="sxs-lookup"><span data-stu-id="54147-150">installStateDetail</span></span>|[<span data-ttu-id="54147-151">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="54147-151">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="54147-152">アプリのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="54147-152">The install state detail of the app.</span></span> <span data-ttu-id="54147-153">可能な値は、`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="54147-153">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="54147-154">errorCode</span><span class="sxs-lookup"><span data-stu-id="54147-154">errorCode</span></span>|<span data-ttu-id="54147-155">Int32</span><span class="sxs-lookup"><span data-stu-id="54147-155">Int32</span></span>|<span data-ttu-id="54147-156">インストールまたはアンインストールの失敗のエラーコード。</span><span class="sxs-lookup"><span data-stu-id="54147-156">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="54147-157">osVersion</span><span class="sxs-lookup"><span data-stu-id="54147-157">osVersion</span></span>|<span data-ttu-id="54147-158">String</span><span class="sxs-lookup"><span data-stu-id="54147-158">String</span></span>|<span data-ttu-id="54147-159">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="54147-159">OS Version</span></span>|
|<span data-ttu-id="54147-160">osDescription</span><span class="sxs-lookup"><span data-stu-id="54147-160">osDescription</span></span>|<span data-ttu-id="54147-161">String</span><span class="sxs-lookup"><span data-stu-id="54147-161">String</span></span>|<span data-ttu-id="54147-162">OS の説明</span><span class="sxs-lookup"><span data-stu-id="54147-162">OS Description</span></span>|
|<span data-ttu-id="54147-163">userName</span><span class="sxs-lookup"><span data-stu-id="54147-163">userName</span></span>|<span data-ttu-id="54147-164">String</span><span class="sxs-lookup"><span data-stu-id="54147-164">String</span></span>|<span data-ttu-id="54147-165">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="54147-165">Device User Name</span></span>|
|<span data-ttu-id="54147-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="54147-166">userPrincipalName</span></span>|<span data-ttu-id="54147-167">文字列</span><span class="sxs-lookup"><span data-stu-id="54147-167">String</span></span>|<span data-ttu-id="54147-168">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="54147-168">User Principal Name</span></span>|
|<span data-ttu-id="54147-169">displayversion</span><span class="sxs-lookup"><span data-stu-id="54147-169">displayVersion</span></span>|<span data-ttu-id="54147-170">String</span><span class="sxs-lookup"><span data-stu-id="54147-170">String</span></span>|<span data-ttu-id="54147-171">アプリケーションの人間の読み取り可能なバージョン</span><span class="sxs-lookup"><span data-stu-id="54147-171">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="54147-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54147-172">Relationships</span></span>
|<span data-ttu-id="54147-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54147-173">Relationship</span></span>|<span data-ttu-id="54147-174">型</span><span class="sxs-lookup"><span data-stu-id="54147-174">Type</span></span>|<span data-ttu-id="54147-175">説明</span><span class="sxs-lookup"><span data-stu-id="54147-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54147-176">アプリ</span><span class="sxs-lookup"><span data-stu-id="54147-176">app</span></span>|[<span data-ttu-id="54147-177">mobileApp</span><span class="sxs-lookup"><span data-stu-id="54147-177">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="54147-178">モバイルアプリへのナビゲーションリンク。</span><span class="sxs-lookup"><span data-stu-id="54147-178">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54147-179">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54147-179">JSON Representation</span></span>
<span data-ttu-id="54147-180">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54147-180">Here is a JSON representation of the resource.</span></span>
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




