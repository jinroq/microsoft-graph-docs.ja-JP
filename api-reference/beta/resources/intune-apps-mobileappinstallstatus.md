---
title: mobileAppInstallStatus リソースの種類
description: デバイスのモバイル アプリケーションのインストール状態のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cac5c94f0669f784bf4cdd020448e40799d53915
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982611"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="65bbc-103">mobileAppInstallStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65bbc-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="65bbc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65bbc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65bbc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65bbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65bbc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="65bbc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65bbc-107">デバイスのモバイル アプリケーションのインストール状態のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="65bbc-107">Contains properties for the installation state of a mobile app for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="65bbc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="65bbc-108">Methods</span></span>
|<span data-ttu-id="65bbc-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="65bbc-109">Method</span></span>|<span data-ttu-id="65bbc-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="65bbc-110">Return Type</span></span>|<span data-ttu-id="65bbc-111">説明</span><span class="sxs-lookup"><span data-stu-id="65bbc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65bbc-112">リスト mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="65bbc-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="65bbc-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65bbc-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="65bbc-114">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="65bbc-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="65bbc-115">MobileAppInstallStatus を取得します。</span><span class="sxs-lookup"><span data-stu-id="65bbc-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="65bbc-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="65bbc-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="65bbc-117">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65bbc-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="65bbc-118">MobileAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="65bbc-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="65bbc-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="65bbc-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="65bbc-120">新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="65bbc-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="65bbc-121">MobileAppInstallStatus を削除します。</span><span class="sxs-lookup"><span data-stu-id="65bbc-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="65bbc-122">なし</span><span class="sxs-lookup"><span data-stu-id="65bbc-122">None</span></span>|<span data-ttu-id="65bbc-123">の[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="65bbc-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="65bbc-124">MobileAppInstallStatus を更新します。</span><span class="sxs-lookup"><span data-stu-id="65bbc-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="65bbc-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="65bbc-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="65bbc-126">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="65bbc-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="65bbc-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65bbc-127">Properties</span></span>
|<span data-ttu-id="65bbc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65bbc-128">Property</span></span>|<span data-ttu-id="65bbc-129">型</span><span class="sxs-lookup"><span data-stu-id="65bbc-129">Type</span></span>|<span data-ttu-id="65bbc-130">説明</span><span class="sxs-lookup"><span data-stu-id="65bbc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65bbc-131">ID</span><span class="sxs-lookup"><span data-stu-id="65bbc-131">id</span></span>|<span data-ttu-id="65bbc-132">String</span><span class="sxs-lookup"><span data-stu-id="65bbc-132">String</span></span>|<span data-ttu-id="65bbc-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="65bbc-133">Key of the entity.</span></span>|
|<span data-ttu-id="65bbc-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="65bbc-134">deviceName</span></span>|<span data-ttu-id="65bbc-135">String</span><span class="sxs-lookup"><span data-stu-id="65bbc-135">String</span></span>|<span data-ttu-id="65bbc-136">デバイス名</span><span class="sxs-lookup"><span data-stu-id="65bbc-136">Device name</span></span>|
|<span data-ttu-id="65bbc-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="65bbc-137">deviceId</span></span>|<span data-ttu-id="65bbc-138">String</span><span class="sxs-lookup"><span data-stu-id="65bbc-138">String</span></span>|<span data-ttu-id="65bbc-139">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="65bbc-139">Device ID</span></span>|
|<span data-ttu-id="65bbc-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="65bbc-140">lastSyncDateTime</span></span>|<span data-ttu-id="65bbc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65bbc-141">DateTimeOffset</span></span>|<span data-ttu-id="65bbc-142">前回の同期日時</span><span class="sxs-lookup"><span data-stu-id="65bbc-142">Last sync date time</span></span>|
|<span data-ttu-id="65bbc-143">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="65bbc-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="65bbc-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="65bbc-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="65bbc-145">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="65bbc-145">The install state of the app.</span></span> <span data-ttu-id="65bbc-146">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="65bbc-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="65bbc-147">installState</span><span class="sxs-lookup"><span data-stu-id="65bbc-147">installState</span></span>|[<span data-ttu-id="65bbc-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="65bbc-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="65bbc-149">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="65bbc-149">The install state of the app.</span></span> <span data-ttu-id="65bbc-150">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="65bbc-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="65bbc-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="65bbc-151">installStateDetail</span></span>|[<span data-ttu-id="65bbc-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="65bbc-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="65bbc-153">アプリケーションのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="65bbc-153">The install state detail of the app.</span></span> <span data-ttu-id="65bbc-154">可能な値は、`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="65bbc-154">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="65bbc-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="65bbc-155">errorCode</span></span>|<span data-ttu-id="65bbc-156">Int32</span><span class="sxs-lookup"><span data-stu-id="65bbc-156">Int32</span></span>|<span data-ttu-id="65bbc-157">エラーは、インストール用のコードか、障害をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="65bbc-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="65bbc-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="65bbc-158">osVersion</span></span>|<span data-ttu-id="65bbc-159">String</span><span class="sxs-lookup"><span data-stu-id="65bbc-159">String</span></span>|<span data-ttu-id="65bbc-160">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="65bbc-160">OS Version</span></span>|
|<span data-ttu-id="65bbc-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="65bbc-161">osDescription</span></span>|<span data-ttu-id="65bbc-162">String</span><span class="sxs-lookup"><span data-stu-id="65bbc-162">String</span></span>|<span data-ttu-id="65bbc-163">OS の説明</span><span class="sxs-lookup"><span data-stu-id="65bbc-163">OS Description</span></span>|
|<span data-ttu-id="65bbc-164">userName</span><span class="sxs-lookup"><span data-stu-id="65bbc-164">userName</span></span>|<span data-ttu-id="65bbc-165">String</span><span class="sxs-lookup"><span data-stu-id="65bbc-165">String</span></span>|<span data-ttu-id="65bbc-166">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="65bbc-166">Device User Name</span></span>|
|<span data-ttu-id="65bbc-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65bbc-167">userPrincipalName</span></span>|<span data-ttu-id="65bbc-168">String</span><span class="sxs-lookup"><span data-stu-id="65bbc-168">String</span></span>|<span data-ttu-id="65bbc-169">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="65bbc-169">User Principal Name</span></span>|
|<span data-ttu-id="65bbc-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="65bbc-170">displayVersion</span></span>|<span data-ttu-id="65bbc-171">String</span><span class="sxs-lookup"><span data-stu-id="65bbc-171">String</span></span>|<span data-ttu-id="65bbc-172">人間の読み取り可能なバージョンのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="65bbc-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="65bbc-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65bbc-173">Relationships</span></span>
|<span data-ttu-id="65bbc-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65bbc-174">Relationship</span></span>|<span data-ttu-id="65bbc-175">型</span><span class="sxs-lookup"><span data-stu-id="65bbc-175">Type</span></span>|<span data-ttu-id="65bbc-176">説明</span><span class="sxs-lookup"><span data-stu-id="65bbc-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65bbc-177">アプリ</span><span class="sxs-lookup"><span data-stu-id="65bbc-177">app</span></span>|[<span data-ttu-id="65bbc-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="65bbc-178">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="65bbc-179">モバイル アプリケーションへのナビゲーション リンクです。</span><span class="sxs-lookup"><span data-stu-id="65bbc-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65bbc-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65bbc-180">JSON Representation</span></span>
<span data-ttu-id="65bbc-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65bbc-181">Here is a JSON representation of the resource.</span></span>
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





