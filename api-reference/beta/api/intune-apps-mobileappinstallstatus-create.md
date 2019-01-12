---
title: MobileAppInstallStatus を作成します。
description: 新しい mobileAppInstallStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2425ee773068eea2446b19534f907f48a43fe5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970767"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="d9ab6-103">MobileAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="d9ab6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9ab6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9ab6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9ab6-107">新しい[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9ab6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d9ab6-108">Prerequisites</span></span>
<span data-ttu-id="d9ab6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ab6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9ab6-111">Permission type</span></span>|<span data-ttu-id="d9ab6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9ab6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9ab6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9ab6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9ab6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ab6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9ab6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9ab6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9ab6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-116">Not supported.</span></span>|
|<span data-ttu-id="d9ab6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9ab6-117">Application</span></span>|<span data-ttu-id="d9ab6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9ab6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9ab6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d9ab6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9ab6-120">Request headers</span></span>
|<span data-ttu-id="d9ab6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9ab6-121">Header</span></span>|<span data-ttu-id="d9ab6-122">値</span><span class="sxs-lookup"><span data-stu-id="d9ab6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9ab6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9ab6-123">Authorization</span></span>|<span data-ttu-id="d9ab6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9ab6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9ab6-125">Accept</span></span>|<span data-ttu-id="d9ab6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9ab6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9ab6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9ab6-127">Request body</span></span>
<span data-ttu-id="d9ab6-128">要求の本文に mobileAppInstallStatus オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="d9ab6-129">次の表は、mobileAppInstallStatus を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="d9ab6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9ab6-130">Property</span></span>|<span data-ttu-id="d9ab6-131">型</span><span class="sxs-lookup"><span data-stu-id="d9ab6-131">Type</span></span>|<span data-ttu-id="d9ab6-132">説明</span><span class="sxs-lookup"><span data-stu-id="d9ab6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ab6-133">ID</span><span class="sxs-lookup"><span data-stu-id="d9ab6-133">id</span></span>|<span data-ttu-id="d9ab6-134">String</span><span class="sxs-lookup"><span data-stu-id="d9ab6-134">String</span></span>|<span data-ttu-id="d9ab6-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-135">Key of the entity.</span></span>|
|<span data-ttu-id="d9ab6-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="d9ab6-136">deviceName</span></span>|<span data-ttu-id="d9ab6-137">String</span><span class="sxs-lookup"><span data-stu-id="d9ab6-137">String</span></span>|<span data-ttu-id="d9ab6-138">デバイス名</span><span class="sxs-lookup"><span data-stu-id="d9ab6-138">Device name</span></span>|
|<span data-ttu-id="d9ab6-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="d9ab6-139">deviceId</span></span>|<span data-ttu-id="d9ab6-140">String</span><span class="sxs-lookup"><span data-stu-id="d9ab6-140">String</span></span>|<span data-ttu-id="d9ab6-141">デバイス ID</span><span class="sxs-lookup"><span data-stu-id="d9ab6-141">Device ID</span></span>|
|<span data-ttu-id="d9ab6-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d9ab6-142">lastSyncDateTime</span></span>|<span data-ttu-id="d9ab6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9ab6-143">DateTimeOffset</span></span>|<span data-ttu-id="d9ab6-144">前回の同期日時</span><span class="sxs-lookup"><span data-stu-id="d9ab6-144">Last sync date time</span></span>|
|<span data-ttu-id="d9ab6-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="d9ab6-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="d9ab6-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d9ab6-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d9ab6-147">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-147">The install state of the app.</span></span> <span data-ttu-id="d9ab6-148">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d9ab6-149">installState</span><span class="sxs-lookup"><span data-stu-id="d9ab6-149">installState</span></span>|[<span data-ttu-id="d9ab6-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d9ab6-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d9ab6-151">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-151">The install state of the app.</span></span> <span data-ttu-id="d9ab6-152">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d9ab6-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="d9ab6-153">installStateDetail</span></span>|[<span data-ttu-id="d9ab6-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="d9ab6-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="d9ab6-155">アプリケーションのインストール状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-155">The install state detail of the app.</span></span> <span data-ttu-id="d9ab6-156">可能な値は、`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="d9ab6-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="d9ab6-157">errorCode</span></span>|<span data-ttu-id="d9ab6-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d9ab6-158">Int32</span></span>|<span data-ttu-id="d9ab6-159">エラーは、インストール用のコードか、障害をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="d9ab6-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="d9ab6-160">osVersion</span></span>|<span data-ttu-id="d9ab6-161">String</span><span class="sxs-lookup"><span data-stu-id="d9ab6-161">String</span></span>|<span data-ttu-id="d9ab6-162">OS のバージョン</span><span class="sxs-lookup"><span data-stu-id="d9ab6-162">OS Version</span></span>|
|<span data-ttu-id="d9ab6-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="d9ab6-163">osDescription</span></span>|<span data-ttu-id="d9ab6-164">String</span><span class="sxs-lookup"><span data-stu-id="d9ab6-164">String</span></span>|<span data-ttu-id="d9ab6-165">OS の説明</span><span class="sxs-lookup"><span data-stu-id="d9ab6-165">OS Description</span></span>|
|<span data-ttu-id="d9ab6-166">userName</span><span class="sxs-lookup"><span data-stu-id="d9ab6-166">userName</span></span>|<span data-ttu-id="d9ab6-167">String</span><span class="sxs-lookup"><span data-stu-id="d9ab6-167">String</span></span>|<span data-ttu-id="d9ab6-168">デバイスのユーザー名</span><span class="sxs-lookup"><span data-stu-id="d9ab6-168">Device User Name</span></span>|
|<span data-ttu-id="d9ab6-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d9ab6-169">userPrincipalName</span></span>|<span data-ttu-id="d9ab6-170">String</span><span class="sxs-lookup"><span data-stu-id="d9ab6-170">String</span></span>|<span data-ttu-id="d9ab6-171">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="d9ab6-171">User Principal Name</span></span>|
|<span data-ttu-id="d9ab6-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="d9ab6-172">displayVersion</span></span>|<span data-ttu-id="d9ab6-173">String</span><span class="sxs-lookup"><span data-stu-id="d9ab6-173">String</span></span>|<span data-ttu-id="d9ab6-174">人間の読み取り可能なバージョンのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9ab6-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="d9ab6-175">応答</span><span class="sxs-lookup"><span data-stu-id="d9ab6-175">Response</span></span>
<span data-ttu-id="d9ab6-176">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9ab6-177">例</span><span class="sxs-lookup"><span data-stu-id="d9ab6-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9ab6-178">要求</span><span class="sxs-lookup"><span data-stu-id="d9ab6-178">Request</span></span>
<span data-ttu-id="d9ab6-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9ab6-180">応答</span><span class="sxs-lookup"><span data-stu-id="d9ab6-180">Response</span></span>
<span data-ttu-id="d9ab6-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d9ab6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





