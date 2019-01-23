---
title: mobileAppInstallStatus リソースの種類
description: デバイスのモバイル アプリケーションのインストール状態のプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f9ee188190e834016e7dc919c6a2c672d5e22227
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422433"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="e21a8-103">mobileAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e21a8-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="e21a8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e21a8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e21a8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e21a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e21a8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e21a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e21a8-107">デバイスのモバイル アプリケーションのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e21a8-107">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="e21a8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e21a8-108">Methods</span></span>
|<span data-ttu-id="e21a8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e21a8-109">Method</span></span>|<span data-ttu-id="e21a8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e21a8-110">Return Type</span></span>|<span data-ttu-id="e21a8-111">説明</span><span class="sxs-lookup"><span data-stu-id="e21a8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e21a8-112">リスト mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="e21a8-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="e21a8-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e21a8-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="e21a8-114">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e21a8-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="e21a8-115">MobileAppInstallStatus を取得します。</span><span class="sxs-lookup"><span data-stu-id="e21a8-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="e21a8-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e21a8-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e21a8-117">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e21a8-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e21a8-118">MobileAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="e21a8-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="e21a8-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e21a8-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e21a8-120">新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e21a8-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e21a8-121">MobileAppInstallStatus を削除します。</span><span class="sxs-lookup"><span data-stu-id="e21a8-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="e21a8-122">なし</span><span class="sxs-lookup"><span data-stu-id="e21a8-122">None</span></span>|<span data-ttu-id="e21a8-123">の[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e21a8-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="e21a8-124">MobileAppInstallStatus を更新します。</span><span class="sxs-lookup"><span data-stu-id="e21a8-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="e21a8-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e21a8-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e21a8-126">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e21a8-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e21a8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e21a8-127">Properties</span></span>
|<span data-ttu-id="e21a8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e21a8-128">Property</span></span>|<span data-ttu-id="e21a8-129">型</span><span class="sxs-lookup"><span data-stu-id="e21a8-129">Type</span></span>|<span data-ttu-id="e21a8-130">説明</span><span class="sxs-lookup"><span data-stu-id="e21a8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e21a8-131">id</span><span class="sxs-lookup"><span data-stu-id="e21a8-131">id</span></span>|<span data-ttu-id="e21a8-132">String</span><span class="sxs-lookup"><span data-stu-id="e21a8-132">String</span></span>|<span data-ttu-id="e21a8-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e21a8-133">Key of the entity.</span></span>|
|<span data-ttu-id="e21a8-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="e21a8-134">deviceName</span></span>|<span data-ttu-id="e21a8-135">String</span><span class="sxs-lookup"><span data-stu-id="e21a8-135">String</span></span>|<span data-ttu-id="e21a8-136">デバイス名</span><span class="sxs-lookup"><span data-stu-id="e21a8-136">Device name</span></span>|
|<span data-ttu-id="e21a8-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="e21a8-137">deviceId</span></span>|<span data-ttu-id="e21a8-138">String</span><span class="sxs-lookup"><span data-stu-id="e21a8-138">String</span></span>|<span data-ttu-id="e21a8-139">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="e21a8-139">Device ID</span></span>|
|<span data-ttu-id="e21a8-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e21a8-140">lastSyncDateTime</span></span>|<span data-ttu-id="e21a8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e21a8-141">DateTimeOffset</span></span>|<span data-ttu-id="e21a8-142">前回の同期日時</span><span class="sxs-lookup"><span data-stu-id="e21a8-142">Last sync date time</span></span>|
|<span data-ttu-id="e21a8-143">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="e21a8-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="e21a8-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e21a8-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e21a8-145">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="e21a8-145">The install state of the app.</span></span> <span data-ttu-id="e21a8-146">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="e21a8-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e21a8-147">installState</span><span class="sxs-lookup"><span data-stu-id="e21a8-147">installState</span></span>|[<span data-ttu-id="e21a8-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e21a8-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e21a8-149">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="e21a8-149">The install state of the app.</span></span> <span data-ttu-id="e21a8-150">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="e21a8-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e21a8-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="e21a8-151">installStateDetail</span></span>|[<span data-ttu-id="e21a8-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="e21a8-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="e21a8-153">アプリケーションのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="e21a8-153">The install state detail of the app.</span></span> <span data-ttu-id="e21a8-154">可能な値は、`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="e21a8-154">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="e21a8-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="e21a8-155">errorCode</span></span>|<span data-ttu-id="e21a8-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e21a8-156">Int32</span></span>|<span data-ttu-id="e21a8-157">エラーは、インストール用のコードか、障害をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="e21a8-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="e21a8-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="e21a8-158">osVersion</span></span>|<span data-ttu-id="e21a8-159">String</span><span class="sxs-lookup"><span data-stu-id="e21a8-159">String</span></span>|<span data-ttu-id="e21a8-160">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="e21a8-160">OS Version</span></span>|
|<span data-ttu-id="e21a8-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="e21a8-161">osDescription</span></span>|<span data-ttu-id="e21a8-162">String</span><span class="sxs-lookup"><span data-stu-id="e21a8-162">String</span></span>|<span data-ttu-id="e21a8-163">OS の説明</span><span class="sxs-lookup"><span data-stu-id="e21a8-163">OS Description</span></span>|
|<span data-ttu-id="e21a8-164">userName</span><span class="sxs-lookup"><span data-stu-id="e21a8-164">userName</span></span>|<span data-ttu-id="e21a8-165">String</span><span class="sxs-lookup"><span data-stu-id="e21a8-165">String</span></span>|<span data-ttu-id="e21a8-166">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="e21a8-166">Device User Name</span></span>|
|<span data-ttu-id="e21a8-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e21a8-167">userPrincipalName</span></span>|<span data-ttu-id="e21a8-168">String</span><span class="sxs-lookup"><span data-stu-id="e21a8-168">String</span></span>|<span data-ttu-id="e21a8-169">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="e21a8-169">User Principal Name</span></span>|
|<span data-ttu-id="e21a8-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e21a8-170">displayVersion</span></span>|<span data-ttu-id="e21a8-171">String</span><span class="sxs-lookup"><span data-stu-id="e21a8-171">String</span></span>|<span data-ttu-id="e21a8-172">人間の読み取り可能なバージョンのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="e21a8-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e21a8-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e21a8-173">Relationships</span></span>
|<span data-ttu-id="e21a8-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e21a8-174">Relationship</span></span>|<span data-ttu-id="e21a8-175">型</span><span class="sxs-lookup"><span data-stu-id="e21a8-175">Type</span></span>|<span data-ttu-id="e21a8-176">説明</span><span class="sxs-lookup"><span data-stu-id="e21a8-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e21a8-177">アプリ</span><span class="sxs-lookup"><span data-stu-id="e21a8-177">app</span></span>|[<span data-ttu-id="e21a8-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e21a8-178">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="e21a8-179">モバイル アプリケーションへのナビゲーション リンクです。</span><span class="sxs-lookup"><span data-stu-id="e21a8-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e21a8-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e21a8-180">JSON Representation</span></span>
<span data-ttu-id="e21a8-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e21a8-181">Here is a JSON representation of the resource.</span></span>
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




