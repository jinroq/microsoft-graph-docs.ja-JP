---
title: MobileAppInstallStatus を更新します。
description: MobileAppInstallStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a60bcf69ded37ea0b4a04430c6a837bb6df95100
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817949"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="b230f-103">MobileAppInstallStatus を更新します。</span><span class="sxs-lookup"><span data-stu-id="b230f-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="b230f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b230f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b230f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b230f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b230f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b230f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b230f-107">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b230f-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b230f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b230f-108">Prerequisites</span></span>
<span data-ttu-id="b230f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b230f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b230f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b230f-111">Permission type</span></span>|<span data-ttu-id="b230f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b230f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b230f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b230f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b230f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b230f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b230f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b230f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b230f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b230f-116">Not supported.</span></span>|
|<span data-ttu-id="b230f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b230f-117">Application</span></span>|<span data-ttu-id="b230f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b230f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b230f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b230f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b230f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b230f-120">Request headers</span></span>
|<span data-ttu-id="b230f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b230f-121">Header</span></span>|<span data-ttu-id="b230f-122">値</span><span class="sxs-lookup"><span data-stu-id="b230f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b230f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b230f-123">Authorization</span></span>|<span data-ttu-id="b230f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b230f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b230f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b230f-125">Accept</span></span>|<span data-ttu-id="b230f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b230f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b230f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b230f-127">Request body</span></span>
<span data-ttu-id="b230f-128">要求の本文に[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b230f-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="b230f-129">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="b230f-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="b230f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b230f-130">Property</span></span>|<span data-ttu-id="b230f-131">種類</span><span class="sxs-lookup"><span data-stu-id="b230f-131">Type</span></span>|<span data-ttu-id="b230f-132">説明</span><span class="sxs-lookup"><span data-stu-id="b230f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b230f-133">ID</span><span class="sxs-lookup"><span data-stu-id="b230f-133">id</span></span>|<span data-ttu-id="b230f-134">String</span><span class="sxs-lookup"><span data-stu-id="b230f-134">String</span></span>|<span data-ttu-id="b230f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b230f-135">Key of the entity.</span></span>|
|<span data-ttu-id="b230f-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="b230f-136">deviceName</span></span>|<span data-ttu-id="b230f-137">String</span><span class="sxs-lookup"><span data-stu-id="b230f-137">String</span></span>|<span data-ttu-id="b230f-138">デバイス名</span><span class="sxs-lookup"><span data-stu-id="b230f-138">Device name</span></span>|
|<span data-ttu-id="b230f-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="b230f-139">deviceId</span></span>|<span data-ttu-id="b230f-140">String</span><span class="sxs-lookup"><span data-stu-id="b230f-140">String</span></span>|<span data-ttu-id="b230f-141">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="b230f-141">Device ID</span></span>|
|<span data-ttu-id="b230f-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b230f-142">lastSyncDateTime</span></span>|<span data-ttu-id="b230f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b230f-143">DateTimeOffset</span></span>|<span data-ttu-id="b230f-144">前回の同期日時</span><span class="sxs-lookup"><span data-stu-id="b230f-144">Last sync date time</span></span>|
|<span data-ttu-id="b230f-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="b230f-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="b230f-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="b230f-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="b230f-147">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="b230f-147">The install state of the app.</span></span> <span data-ttu-id="b230f-148">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="b230f-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="b230f-149">installState</span><span class="sxs-lookup"><span data-stu-id="b230f-149">installState</span></span>|[<span data-ttu-id="b230f-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="b230f-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="b230f-151">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="b230f-151">The install state of the app.</span></span> <span data-ttu-id="b230f-152">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="b230f-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="b230f-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="b230f-153">installStateDetail</span></span>|[<span data-ttu-id="b230f-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="b230f-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="b230f-155">アプリケーションのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="b230f-155">The install state detail of the app.</span></span> <span data-ttu-id="b230f-156">可能な値は、`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="b230f-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="b230f-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="b230f-157">errorCode</span></span>|<span data-ttu-id="b230f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b230f-158">Int32</span></span>|<span data-ttu-id="b230f-159">エラーは、インストール用のコードか、障害をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="b230f-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="b230f-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="b230f-160">osVersion</span></span>|<span data-ttu-id="b230f-161">String</span><span class="sxs-lookup"><span data-stu-id="b230f-161">String</span></span>|<span data-ttu-id="b230f-162">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="b230f-162">OS Version</span></span>|
|<span data-ttu-id="b230f-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="b230f-163">osDescription</span></span>|<span data-ttu-id="b230f-164">String</span><span class="sxs-lookup"><span data-stu-id="b230f-164">String</span></span>|<span data-ttu-id="b230f-165">OS の説明</span><span class="sxs-lookup"><span data-stu-id="b230f-165">OS Description</span></span>|
|<span data-ttu-id="b230f-166">userName</span><span class="sxs-lookup"><span data-stu-id="b230f-166">userName</span></span>|<span data-ttu-id="b230f-167">String</span><span class="sxs-lookup"><span data-stu-id="b230f-167">String</span></span>|<span data-ttu-id="b230f-168">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="b230f-168">Device User Name</span></span>|
|<span data-ttu-id="b230f-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b230f-169">userPrincipalName</span></span>|<span data-ttu-id="b230f-170">String</span><span class="sxs-lookup"><span data-stu-id="b230f-170">String</span></span>|<span data-ttu-id="b230f-171">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="b230f-171">User Principal Name</span></span>|
|<span data-ttu-id="b230f-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="b230f-172">displayVersion</span></span>|<span data-ttu-id="b230f-173">String</span><span class="sxs-lookup"><span data-stu-id="b230f-173">String</span></span>|<span data-ttu-id="b230f-174">人間の読み取り可能なバージョンのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="b230f-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="b230f-175">応答</span><span class="sxs-lookup"><span data-stu-id="b230f-175">Response</span></span>
<span data-ttu-id="b230f-176">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b230f-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b230f-177">例</span><span class="sxs-lookup"><span data-stu-id="b230f-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="b230f-178">要求</span><span class="sxs-lookup"><span data-stu-id="b230f-178">Request</span></span>
<span data-ttu-id="b230f-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b230f-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 488

{
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

### <a name="response"></a><span data-ttu-id="b230f-180">応答</span><span class="sxs-lookup"><span data-stu-id="b230f-180">Response</span></span>
<span data-ttu-id="b230f-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b230f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





