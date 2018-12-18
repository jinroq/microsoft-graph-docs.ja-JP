---
title: iosUpdateDeviceStatus の作成
description: 新しい iosUpdateDeviceStatus オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 7927912d236058128a9e5263d1d6a9090ce394a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358150"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="2d2e0-103">iosUpdateDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="2d2e0-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="2d2e0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d2e0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d2e0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d2e0-107">新しい [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d2e0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d2e0-108">Prerequisites</span></span>
<span data-ttu-id="2d2e0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d2e0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d2e0-111">Permission type</span></span>|<span data-ttu-id="2d2e0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d2e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d2e0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d2e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d2e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d2e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d2e0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d2e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d2e0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-116">Not supported.</span></span>|
|<span data-ttu-id="2d2e0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d2e0-117">Application</span></span>|<span data-ttu-id="2d2e0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d2e0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d2e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2d2e0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d2e0-120">Request headers</span></span>
|<span data-ttu-id="2d2e0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d2e0-121">Header</span></span>|<span data-ttu-id="2d2e0-122">値</span><span class="sxs-lookup"><span data-stu-id="2d2e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d2e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d2e0-123">Authorization</span></span>|<span data-ttu-id="2d2e0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d2e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2d2e0-125">Accept</span></span>|<span data-ttu-id="2d2e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d2e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d2e0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d2e0-127">Request body</span></span>
<span data-ttu-id="2d2e0-128">要求本文で、iosUpdateDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="2d2e0-129">次の表に、iosUpdateDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="2d2e0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d2e0-130">Property</span></span>|<span data-ttu-id="2d2e0-131">種類</span><span class="sxs-lookup"><span data-stu-id="2d2e0-131">Type</span></span>|<span data-ttu-id="2d2e0-132">説明</span><span class="sxs-lookup"><span data-stu-id="2d2e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d2e0-133">ID</span><span class="sxs-lookup"><span data-stu-id="2d2e0-133">id</span></span>|<span data-ttu-id="2d2e0-134">String</span><span class="sxs-lookup"><span data-stu-id="2d2e0-134">String</span></span>|<span data-ttu-id="2d2e0-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-135">Key of the entity.</span></span>|
|<span data-ttu-id="2d2e0-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="2d2e0-136">installStatus</span></span>|[<span data-ttu-id="2d2e0-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2d2e0-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="2d2e0-138">ポリシー レポートのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-138">The installation status of the policy report.</span></span> <span data-ttu-id="2d2e0-139">使用可能な値: `success`、 `available`、 `idle`、 `unknown`、 `downloading`、 `downloadFailed`、 `downloadRequiresComputer`、 `downloadInsufficientSpace`、 `downloadInsufficientPower`、 `downloadInsufficientNetwork`、 `installing`、 `installInsufficientSpace`、 `installInsufficientPower`、 `installPhoneCallInProgress`、 `installFailed`、 `notSupportedOperation`、 `sharedDeviceUserLoggedInError`。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="2d2e0-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="2d2e0-140">osVersion</span></span>|<span data-ttu-id="2d2e0-141">String</span><span class="sxs-lookup"><span data-stu-id="2d2e0-141">String</span></span>|<span data-ttu-id="2d2e0-142">レポートされているデバイス バージョン。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="2d2e0-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="2d2e0-143">deviceId</span></span>|<span data-ttu-id="2d2e0-144">String</span><span class="sxs-lookup"><span data-stu-id="2d2e0-144">String</span></span>|<span data-ttu-id="2d2e0-145">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="2d2e0-146">userId</span><span class="sxs-lookup"><span data-stu-id="2d2e0-146">userId</span></span>|<span data-ttu-id="2d2e0-147">String</span><span class="sxs-lookup"><span data-stu-id="2d2e0-147">String</span></span>|<span data-ttu-id="2d2e0-148">レポートされているユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="2d2e0-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2d2e0-149">deviceDisplayName</span></span>|<span data-ttu-id="2d2e0-150">String</span><span class="sxs-lookup"><span data-stu-id="2d2e0-150">String</span></span>|<span data-ttu-id="2d2e0-151">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2d2e0-152">userName</span><span class="sxs-lookup"><span data-stu-id="2d2e0-152">userName</span></span>|<span data-ttu-id="2d2e0-153">String</span><span class="sxs-lookup"><span data-stu-id="2d2e0-153">String</span></span>|<span data-ttu-id="2d2e0-154">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="2d2e0-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="2d2e0-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2d2e0-155">deviceModel</span></span>|<span data-ttu-id="2d2e0-156">String</span><span class="sxs-lookup"><span data-stu-id="2d2e0-156">String</span></span>|<span data-ttu-id="2d2e0-157">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="2d2e0-157">The device model that is being reported</span></span>|
|<span data-ttu-id="2d2e0-158">platform</span><span class="sxs-lookup"><span data-stu-id="2d2e0-158">platform</span></span>|<span data-ttu-id="2d2e0-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2d2e0-159">Int32</span></span>|<span data-ttu-id="2d2e0-160">報告されているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="2d2e0-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="2d2e0-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2d2e0-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2d2e0-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d2e0-162">DateTimeOffset</span></span>|<span data-ttu-id="2d2e0-163">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="2d2e0-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2d2e0-164">status</span><span class="sxs-lookup"><span data-stu-id="2d2e0-164">status</span></span>|[<span data-ttu-id="2d2e0-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2d2e0-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2d2e0-166">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-166">Compliance status of the policy report.</span></span> <span data-ttu-id="2d2e0-167">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2d2e0-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d2e0-168">lastReportedDateTime</span></span>|<span data-ttu-id="2d2e0-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d2e0-169">DateTimeOffset</span></span>|<span data-ttu-id="2d2e0-170">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2d2e0-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2d2e0-171">userPrincipalName</span></span>|<span data-ttu-id="2d2e0-172">String</span><span class="sxs-lookup"><span data-stu-id="2d2e0-172">String</span></span>|<span data-ttu-id="2d2e0-173">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2d2e0-174">応答</span><span class="sxs-lookup"><span data-stu-id="2d2e0-174">Response</span></span>
<span data-ttu-id="2d2e0-175">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d2e0-176">例</span><span class="sxs-lookup"><span data-stu-id="2d2e0-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d2e0-177">要求</span><span class="sxs-lookup"><span data-stu-id="2d2e0-177">Request</span></span>
<span data-ttu-id="2d2e0-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="2d2e0-179">応答</span><span class="sxs-lookup"><span data-stu-id="2d2e0-179">Response</span></span>
<span data-ttu-id="2d2e0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d2e0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 619

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





