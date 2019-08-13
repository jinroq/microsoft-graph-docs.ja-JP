---
title: MobileAppInstallStatus の更新
description: MobileAppInstallStatus オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89c61d75ee7299bc942f82d9a4ccf209bc70d6bc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336489"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="aa437-103">MobileAppInstallStatus の更新</span><span class="sxs-lookup"><span data-stu-id="aa437-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="aa437-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa437-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa437-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa437-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa437-106">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa437-106">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa437-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="aa437-107">Prerequisites</span></span>
<span data-ttu-id="aa437-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa437-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aa437-110">Permission type</span></span>|<span data-ttu-id="aa437-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aa437-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa437-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aa437-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa437-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa437-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aa437-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aa437-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa437-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa437-115">Not supported.</span></span>|
|<span data-ttu-id="aa437-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aa437-116">Application</span></span>|<span data-ttu-id="aa437-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa437-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa437-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aa437-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="aa437-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa437-119">Request headers</span></span>
|<span data-ttu-id="aa437-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa437-120">Header</span></span>|<span data-ttu-id="aa437-121">値</span><span class="sxs-lookup"><span data-stu-id="aa437-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa437-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa437-122">Authorization</span></span>|<span data-ttu-id="aa437-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa437-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa437-124">承諾</span><span class="sxs-lookup"><span data-stu-id="aa437-124">Accept</span></span>|<span data-ttu-id="aa437-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa437-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa437-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="aa437-126">Request body</span></span>
<span data-ttu-id="aa437-127">要求本文で、 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="aa437-127">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="aa437-128">次の表に、 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="aa437-128">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="aa437-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa437-129">Property</span></span>|<span data-ttu-id="aa437-130">型</span><span class="sxs-lookup"><span data-stu-id="aa437-130">Type</span></span>|<span data-ttu-id="aa437-131">説明</span><span class="sxs-lookup"><span data-stu-id="aa437-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa437-132">id</span><span class="sxs-lookup"><span data-stu-id="aa437-132">id</span></span>|<span data-ttu-id="aa437-133">文字列</span><span class="sxs-lookup"><span data-stu-id="aa437-133">String</span></span>|<span data-ttu-id="aa437-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aa437-134">Key of the entity.</span></span>|
|<span data-ttu-id="aa437-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="aa437-135">deviceName</span></span>|<span data-ttu-id="aa437-136">String</span><span class="sxs-lookup"><span data-stu-id="aa437-136">String</span></span>|<span data-ttu-id="aa437-137">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="aa437-137">Device name</span></span>|
|<span data-ttu-id="aa437-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="aa437-138">deviceId</span></span>|<span data-ttu-id="aa437-139">String</span><span class="sxs-lookup"><span data-stu-id="aa437-139">String</span></span>|<span data-ttu-id="aa437-140">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="aa437-140">Device ID</span></span>|
|<span data-ttu-id="aa437-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="aa437-141">lastSyncDateTime</span></span>|<span data-ttu-id="aa437-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa437-142">DateTimeOffset</span></span>|<span data-ttu-id="aa437-143">最終同期日時</span><span class="sxs-lookup"><span data-stu-id="aa437-143">Last sync date time</span></span>|
|<span data-ttu-id="aa437-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="aa437-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="aa437-145">Resultappstate</span><span class="sxs-lookup"><span data-stu-id="aa437-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="aa437-146">アプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="aa437-146">The install state of the app.</span></span> <span data-ttu-id="aa437-147">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="aa437-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="aa437-148">installState</span><span class="sxs-lookup"><span data-stu-id="aa437-148">installState</span></span>|[<span data-ttu-id="aa437-149">Resultappstate</span><span class="sxs-lookup"><span data-stu-id="aa437-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="aa437-150">アプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="aa437-150">The install state of the app.</span></span> <span data-ttu-id="aa437-151">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="aa437-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="aa437-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="aa437-152">installStateDetail</span></span>|[<span data-ttu-id="aa437-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="aa437-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="aa437-154">アプリのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="aa437-154">The install state detail of the app.</span></span> <span data-ttu-id="aa437-155">可能な値: `noAdditionalDetails`、 `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`、、、、、、、、、、、、 `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="aa437-155">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="aa437-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="aa437-156">errorCode</span></span>|<span data-ttu-id="aa437-157">Int32</span><span class="sxs-lookup"><span data-stu-id="aa437-157">Int32</span></span>|<span data-ttu-id="aa437-158">インストールまたはアンインストールの失敗のエラーコード。</span><span class="sxs-lookup"><span data-stu-id="aa437-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="aa437-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="aa437-159">osVersion</span></span>|<span data-ttu-id="aa437-160">String</span><span class="sxs-lookup"><span data-stu-id="aa437-160">String</span></span>|<span data-ttu-id="aa437-161">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="aa437-161">OS Version</span></span>|
|<span data-ttu-id="aa437-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="aa437-162">osDescription</span></span>|<span data-ttu-id="aa437-163">String</span><span class="sxs-lookup"><span data-stu-id="aa437-163">String</span></span>|<span data-ttu-id="aa437-164">OS の説明</span><span class="sxs-lookup"><span data-stu-id="aa437-164">OS Description</span></span>|
|<span data-ttu-id="aa437-165">userName</span><span class="sxs-lookup"><span data-stu-id="aa437-165">userName</span></span>|<span data-ttu-id="aa437-166">String</span><span class="sxs-lookup"><span data-stu-id="aa437-166">String</span></span>|<span data-ttu-id="aa437-167">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="aa437-167">Device User Name</span></span>|
|<span data-ttu-id="aa437-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aa437-168">userPrincipalName</span></span>|<span data-ttu-id="aa437-169">String</span><span class="sxs-lookup"><span data-stu-id="aa437-169">String</span></span>|<span data-ttu-id="aa437-170">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="aa437-170">User Principal Name</span></span>|
|<span data-ttu-id="aa437-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="aa437-171">displayVersion</span></span>|<span data-ttu-id="aa437-172">String</span><span class="sxs-lookup"><span data-stu-id="aa437-172">String</span></span>|<span data-ttu-id="aa437-173">アプリケーションの人間の読み取り可能なバージョン</span><span class="sxs-lookup"><span data-stu-id="aa437-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="aa437-174">応答</span><span class="sxs-lookup"><span data-stu-id="aa437-174">Response</span></span>
<span data-ttu-id="aa437-175">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aa437-175">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa437-176">例</span><span class="sxs-lookup"><span data-stu-id="aa437-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa437-177">要求</span><span class="sxs-lookup"><span data-stu-id="aa437-177">Request</span></span>
<span data-ttu-id="aa437-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aa437-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "dependencyFailedToInstall",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="aa437-179">応答</span><span class="sxs-lookup"><span data-stu-id="aa437-179">Response</span></span>
<span data-ttu-id="aa437-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa437-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 604

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "dependencyFailedToInstall",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```






