---
title: mobileAppInstallStatus リソースの種類
description: デバイスのモバイル アプリケーションのインストール状態のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: ba2c0026d54235683a2f5d5b26c19b88ea11a9d6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320889"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="47cd6-103">mobileAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47cd6-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="47cd6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47cd6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47cd6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47cd6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47cd6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="47cd6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47cd6-107">デバイスのモバイル アプリケーションのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="47cd6-107">Contains properties for the installation state of a mobile app for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="47cd6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="47cd6-108">Methods</span></span>
|<span data-ttu-id="47cd6-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="47cd6-109">Method</span></span>|<span data-ttu-id="47cd6-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="47cd6-110">Return Type</span></span>|<span data-ttu-id="47cd6-111">説明</span><span class="sxs-lookup"><span data-stu-id="47cd6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47cd6-112">リスト mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="47cd6-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="47cd6-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="47cd6-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="47cd6-114">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="47cd6-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="47cd6-115">MobileAppInstallStatus を取得します。</span><span class="sxs-lookup"><span data-stu-id="47cd6-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="47cd6-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="47cd6-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="47cd6-117">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47cd6-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="47cd6-118">MobileAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="47cd6-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="47cd6-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="47cd6-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="47cd6-120">新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="47cd6-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="47cd6-121">MobileAppInstallStatus を削除します。</span><span class="sxs-lookup"><span data-stu-id="47cd6-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="47cd6-122">なし</span><span class="sxs-lookup"><span data-stu-id="47cd6-122">None</span></span>|<span data-ttu-id="47cd6-123">の[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="47cd6-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="47cd6-124">MobileAppInstallStatus を更新します。</span><span class="sxs-lookup"><span data-stu-id="47cd6-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="47cd6-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="47cd6-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="47cd6-126">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="47cd6-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47cd6-127">Properties</span><span class="sxs-lookup"><span data-stu-id="47cd6-127">Properties</span></span>
|<span data-ttu-id="47cd6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47cd6-128">Property</span></span>|<span data-ttu-id="47cd6-129">種類</span><span class="sxs-lookup"><span data-stu-id="47cd6-129">Type</span></span>|<span data-ttu-id="47cd6-130">説明</span><span class="sxs-lookup"><span data-stu-id="47cd6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47cd6-131">ID</span><span class="sxs-lookup"><span data-stu-id="47cd6-131">id</span></span>|<span data-ttu-id="47cd6-132">String</span><span class="sxs-lookup"><span data-stu-id="47cd6-132">String</span></span>|<span data-ttu-id="47cd6-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="47cd6-133">Key of the entity.</span></span>|
|<span data-ttu-id="47cd6-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="47cd6-134">deviceName</span></span>|<span data-ttu-id="47cd6-135">String</span><span class="sxs-lookup"><span data-stu-id="47cd6-135">String</span></span>|<span data-ttu-id="47cd6-136">デバイス名</span><span class="sxs-lookup"><span data-stu-id="47cd6-136">Device name</span></span>|
|<span data-ttu-id="47cd6-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="47cd6-137">deviceId</span></span>|<span data-ttu-id="47cd6-138">String</span><span class="sxs-lookup"><span data-stu-id="47cd6-138">String</span></span>|<span data-ttu-id="47cd6-139">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="47cd6-139">Device ID</span></span>|
|<span data-ttu-id="47cd6-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="47cd6-140">lastSyncDateTime</span></span>|<span data-ttu-id="47cd6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47cd6-141">DateTimeOffset</span></span>|<span data-ttu-id="47cd6-142">前回の同期日時</span><span class="sxs-lookup"><span data-stu-id="47cd6-142">Last sync date time</span></span>|
|<span data-ttu-id="47cd6-143">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="47cd6-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="47cd6-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="47cd6-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="47cd6-145">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="47cd6-145">The install state of the app.</span></span> <span data-ttu-id="47cd6-146">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="47cd6-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="47cd6-147">installState</span><span class="sxs-lookup"><span data-stu-id="47cd6-147">installState</span></span>|[<span data-ttu-id="47cd6-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="47cd6-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="47cd6-149">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="47cd6-149">The install state of the app.</span></span> <span data-ttu-id="47cd6-150">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="47cd6-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="47cd6-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="47cd6-151">installStateDetail</span></span>|[<span data-ttu-id="47cd6-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="47cd6-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="47cd6-153">アプリケーションのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="47cd6-153">The install state detail of the app.</span></span> <span data-ttu-id="47cd6-154">可能な値は、`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="47cd6-154">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="47cd6-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="47cd6-155">errorCode</span></span>|<span data-ttu-id="47cd6-156">Int32</span><span class="sxs-lookup"><span data-stu-id="47cd6-156">Int32</span></span>|<span data-ttu-id="47cd6-157">エラーは、インストール用のコードか、障害をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="47cd6-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="47cd6-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="47cd6-158">osVersion</span></span>|<span data-ttu-id="47cd6-159">String</span><span class="sxs-lookup"><span data-stu-id="47cd6-159">String</span></span>|<span data-ttu-id="47cd6-160">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="47cd6-160">OS Version</span></span>|
|<span data-ttu-id="47cd6-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="47cd6-161">osDescription</span></span>|<span data-ttu-id="47cd6-162">String</span><span class="sxs-lookup"><span data-stu-id="47cd6-162">String</span></span>|<span data-ttu-id="47cd6-163">OS の説明</span><span class="sxs-lookup"><span data-stu-id="47cd6-163">OS Description</span></span>|
|<span data-ttu-id="47cd6-164">userName</span><span class="sxs-lookup"><span data-stu-id="47cd6-164">userName</span></span>|<span data-ttu-id="47cd6-165">String</span><span class="sxs-lookup"><span data-stu-id="47cd6-165">String</span></span>|<span data-ttu-id="47cd6-166">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="47cd6-166">Device User Name</span></span>|
|<span data-ttu-id="47cd6-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="47cd6-167">userPrincipalName</span></span>|<span data-ttu-id="47cd6-168">String</span><span class="sxs-lookup"><span data-stu-id="47cd6-168">String</span></span>|<span data-ttu-id="47cd6-169">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="47cd6-169">User Principal Name</span></span>|
|<span data-ttu-id="47cd6-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="47cd6-170">displayVersion</span></span>|<span data-ttu-id="47cd6-171">String</span><span class="sxs-lookup"><span data-stu-id="47cd6-171">String</span></span>|<span data-ttu-id="47cd6-172">人間の読み取り可能なバージョンのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="47cd6-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="47cd6-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47cd6-173">Relationships</span></span>
|<span data-ttu-id="47cd6-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47cd6-174">Relationship</span></span>|<span data-ttu-id="47cd6-175">型</span><span class="sxs-lookup"><span data-stu-id="47cd6-175">Type</span></span>|<span data-ttu-id="47cd6-176">説明</span><span class="sxs-lookup"><span data-stu-id="47cd6-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47cd6-177">アプリ</span><span class="sxs-lookup"><span data-stu-id="47cd6-177">app</span></span>|[<span data-ttu-id="47cd6-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="47cd6-178">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="47cd6-179">モバイル アプリケーションへのナビゲーション リンクです。</span><span class="sxs-lookup"><span data-stu-id="47cd6-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47cd6-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47cd6-180">JSON Representation</span></span>
<span data-ttu-id="47cd6-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47cd6-181">Here is a JSON representation of the resource.</span></span>
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




