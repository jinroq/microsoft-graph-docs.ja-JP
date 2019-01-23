---
title: MobileAppInstallStatus を作成します。
description: 新しい mobileAppInstallStatus オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 123a07d7b7576bfc94011e20d45a6d0c8e65abc0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394195"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="d4417-103">MobileAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="d4417-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="d4417-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d4417-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4417-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4417-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4417-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4417-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4417-107">新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d4417-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4417-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4417-108">Prerequisites</span></span>
<span data-ttu-id="d4417-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d4417-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4417-111">Permission type</span></span>|<span data-ttu-id="d4417-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4417-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4417-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4417-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4417-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4417-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4417-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4417-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4417-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4417-116">Not supported.</span></span>|
|<span data-ttu-id="d4417-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4417-117">Application</span></span>|<span data-ttu-id="d4417-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4417-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4417-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4417-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d4417-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4417-120">Request headers</span></span>
|<span data-ttu-id="d4417-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4417-121">Header</span></span>|<span data-ttu-id="d4417-122">値</span><span class="sxs-lookup"><span data-stu-id="d4417-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4417-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4417-123">Authorization</span></span>|<span data-ttu-id="d4417-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d4417-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4417-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4417-125">Accept</span></span>|<span data-ttu-id="d4417-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4417-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4417-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4417-127">Request body</span></span>
<span data-ttu-id="d4417-128">要求の本文に mobileAppInstallStatus オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d4417-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="d4417-129">次の表は、mobileAppInstallStatus を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d4417-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="d4417-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4417-130">Property</span></span>|<span data-ttu-id="d4417-131">型</span><span class="sxs-lookup"><span data-stu-id="d4417-131">Type</span></span>|<span data-ttu-id="d4417-132">説明</span><span class="sxs-lookup"><span data-stu-id="d4417-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4417-133">id</span><span class="sxs-lookup"><span data-stu-id="d4417-133">id</span></span>|<span data-ttu-id="d4417-134">String</span><span class="sxs-lookup"><span data-stu-id="d4417-134">String</span></span>|<span data-ttu-id="d4417-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d4417-135">Key of the entity.</span></span>|
|<span data-ttu-id="d4417-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="d4417-136">deviceName</span></span>|<span data-ttu-id="d4417-137">String</span><span class="sxs-lookup"><span data-stu-id="d4417-137">String</span></span>|<span data-ttu-id="d4417-138">デバイス名</span><span class="sxs-lookup"><span data-stu-id="d4417-138">Device name</span></span>|
|<span data-ttu-id="d4417-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="d4417-139">deviceId</span></span>|<span data-ttu-id="d4417-140">String</span><span class="sxs-lookup"><span data-stu-id="d4417-140">String</span></span>|<span data-ttu-id="d4417-141">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="d4417-141">Device ID</span></span>|
|<span data-ttu-id="d4417-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d4417-142">lastSyncDateTime</span></span>|<span data-ttu-id="d4417-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4417-143">DateTimeOffset</span></span>|<span data-ttu-id="d4417-144">前回の同期日時</span><span class="sxs-lookup"><span data-stu-id="d4417-144">Last sync date time</span></span>|
|<span data-ttu-id="d4417-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="d4417-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="d4417-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d4417-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d4417-147">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="d4417-147">The install state of the app.</span></span> <span data-ttu-id="d4417-148">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="d4417-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d4417-149">installState</span><span class="sxs-lookup"><span data-stu-id="d4417-149">installState</span></span>|[<span data-ttu-id="d4417-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d4417-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d4417-151">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="d4417-151">The install state of the app.</span></span> <span data-ttu-id="d4417-152">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="d4417-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d4417-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="d4417-153">installStateDetail</span></span>|[<span data-ttu-id="d4417-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="d4417-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="d4417-155">アプリケーションのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="d4417-155">The install state detail of the app.</span></span> <span data-ttu-id="d4417-156">可能な値は、`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="d4417-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="d4417-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="d4417-157">errorCode</span></span>|<span data-ttu-id="d4417-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d4417-158">Int32</span></span>|<span data-ttu-id="d4417-159">エラーは、インストール用のコードか、障害をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="d4417-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="d4417-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="d4417-160">osVersion</span></span>|<span data-ttu-id="d4417-161">String</span><span class="sxs-lookup"><span data-stu-id="d4417-161">String</span></span>|<span data-ttu-id="d4417-162">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="d4417-162">OS Version</span></span>|
|<span data-ttu-id="d4417-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="d4417-163">osDescription</span></span>|<span data-ttu-id="d4417-164">String</span><span class="sxs-lookup"><span data-stu-id="d4417-164">String</span></span>|<span data-ttu-id="d4417-165">OS の説明</span><span class="sxs-lookup"><span data-stu-id="d4417-165">OS Description</span></span>|
|<span data-ttu-id="d4417-166">userName</span><span class="sxs-lookup"><span data-stu-id="d4417-166">userName</span></span>|<span data-ttu-id="d4417-167">String</span><span class="sxs-lookup"><span data-stu-id="d4417-167">String</span></span>|<span data-ttu-id="d4417-168">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="d4417-168">Device User Name</span></span>|
|<span data-ttu-id="d4417-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4417-169">userPrincipalName</span></span>|<span data-ttu-id="d4417-170">String</span><span class="sxs-lookup"><span data-stu-id="d4417-170">String</span></span>|<span data-ttu-id="d4417-171">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="d4417-171">User Principal Name</span></span>|
|<span data-ttu-id="d4417-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="d4417-172">displayVersion</span></span>|<span data-ttu-id="d4417-173">String</span><span class="sxs-lookup"><span data-stu-id="d4417-173">String</span></span>|<span data-ttu-id="d4417-174">人間の読み取り可能なバージョンのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4417-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="d4417-175">応答</span><span class="sxs-lookup"><span data-stu-id="d4417-175">Response</span></span>
<span data-ttu-id="d4417-176">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d4417-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4417-177">例</span><span class="sxs-lookup"><span data-stu-id="d4417-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4417-178">要求</span><span class="sxs-lookup"><span data-stu-id="d4417-178">Request</span></span>
<span data-ttu-id="d4417-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4417-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="d4417-180">応答</span><span class="sxs-lookup"><span data-stu-id="d4417-180">Response</span></span>
<span data-ttu-id="d4417-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4417-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```




