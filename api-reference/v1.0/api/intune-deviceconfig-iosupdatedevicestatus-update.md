---
title: iosUpdateDeviceStatus の更新
description: iosUpdateDeviceStatus オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 623417eb92a557745c9c1d1d04cc5b7f9677bd6c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359305"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="990d8-103">iosUpdateDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="990d8-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="990d8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="990d8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="990d8-105">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="990d8-105">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="990d8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="990d8-106">Prerequisites</span></span>
<span data-ttu-id="990d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="990d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="990d8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="990d8-109">Permission type</span></span>|<span data-ttu-id="990d8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="990d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="990d8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="990d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="990d8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="990d8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="990d8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="990d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="990d8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="990d8-114">Not supported.</span></span>|
|<span data-ttu-id="990d8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="990d8-115">Application</span></span>|<span data-ttu-id="990d8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="990d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="990d8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="990d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="990d8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="990d8-118">Request headers</span></span>
|<span data-ttu-id="990d8-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="990d8-119">Header</span></span>|<span data-ttu-id="990d8-120">値</span><span class="sxs-lookup"><span data-stu-id="990d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="990d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="990d8-121">Authorization</span></span>|<span data-ttu-id="990d8-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="990d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="990d8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="990d8-123">Accept</span></span>|<span data-ttu-id="990d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="990d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="990d8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="990d8-125">Request body</span></span>
<span data-ttu-id="990d8-126">要求本文で、[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="990d8-126">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="990d8-127">次の表に、[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="990d8-127">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="990d8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="990d8-128">Property</span></span>|<span data-ttu-id="990d8-129">種類</span><span class="sxs-lookup"><span data-stu-id="990d8-129">Type</span></span>|<span data-ttu-id="990d8-130">説明</span><span class="sxs-lookup"><span data-stu-id="990d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="990d8-131">ID</span><span class="sxs-lookup"><span data-stu-id="990d8-131">id</span></span>|<span data-ttu-id="990d8-132">String</span><span class="sxs-lookup"><span data-stu-id="990d8-132">String</span></span>|<span data-ttu-id="990d8-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="990d8-133">Key of the entity.</span></span>|
|<span data-ttu-id="990d8-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="990d8-134">installStatus</span></span>|[<span data-ttu-id="990d8-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="990d8-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="990d8-136">ポリシー レポートのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="990d8-136">The installation status of the policy report.</span></span> <span data-ttu-id="990d8-137">使用可能な値: `success`、 `available`、 `idle`、 `unknown`、 `downloading`、 `downloadFailed`、 `downloadRequiresComputer`、 `downloadInsufficientSpace`、 `downloadInsufficientPower`、 `downloadInsufficientNetwork`、 `installing`、 `installInsufficientSpace`、 `installInsufficientPower`、 `installPhoneCallInProgress`、 `installFailed`、 `notSupportedOperation`、 `sharedDeviceUserLoggedInError`。</span><span class="sxs-lookup"><span data-stu-id="990d8-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="990d8-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="990d8-138">osVersion</span></span>|<span data-ttu-id="990d8-139">String</span><span class="sxs-lookup"><span data-stu-id="990d8-139">String</span></span>|<span data-ttu-id="990d8-140">レポートされているデバイス バージョン。</span><span class="sxs-lookup"><span data-stu-id="990d8-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="990d8-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="990d8-141">deviceId</span></span>|<span data-ttu-id="990d8-142">String</span><span class="sxs-lookup"><span data-stu-id="990d8-142">String</span></span>|<span data-ttu-id="990d8-143">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="990d8-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="990d8-144">userId</span><span class="sxs-lookup"><span data-stu-id="990d8-144">userId</span></span>|<span data-ttu-id="990d8-145">String</span><span class="sxs-lookup"><span data-stu-id="990d8-145">String</span></span>|<span data-ttu-id="990d8-146">レポートされているユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="990d8-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="990d8-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="990d8-147">deviceDisplayName</span></span>|<span data-ttu-id="990d8-148">String</span><span class="sxs-lookup"><span data-stu-id="990d8-148">String</span></span>|<span data-ttu-id="990d8-149">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="990d8-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="990d8-150">userName</span><span class="sxs-lookup"><span data-stu-id="990d8-150">userName</span></span>|<span data-ttu-id="990d8-151">String</span><span class="sxs-lookup"><span data-stu-id="990d8-151">String</span></span>|<span data-ttu-id="990d8-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="990d8-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="990d8-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="990d8-153">deviceModel</span></span>|<span data-ttu-id="990d8-154">String</span><span class="sxs-lookup"><span data-stu-id="990d8-154">String</span></span>|<span data-ttu-id="990d8-155">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="990d8-155">The device model that is being reported</span></span>|
|<span data-ttu-id="990d8-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="990d8-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="990d8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="990d8-157">DateTimeOffset</span></span>|<span data-ttu-id="990d8-158">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="990d8-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="990d8-159">status</span><span class="sxs-lookup"><span data-stu-id="990d8-159">status</span></span>|[<span data-ttu-id="990d8-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="990d8-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="990d8-161">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="990d8-161">Compliance status of the policy report.</span></span> <span data-ttu-id="990d8-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="990d8-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="990d8-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="990d8-163">lastReportedDateTime</span></span>|<span data-ttu-id="990d8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="990d8-164">DateTimeOffset</span></span>|<span data-ttu-id="990d8-165">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="990d8-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="990d8-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="990d8-166">userPrincipalName</span></span>|<span data-ttu-id="990d8-167">String</span><span class="sxs-lookup"><span data-stu-id="990d8-167">String</span></span>|<span data-ttu-id="990d8-168">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="990d8-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="990d8-169">応答</span><span class="sxs-lookup"><span data-stu-id="990d8-169">Response</span></span>
<span data-ttu-id="990d8-170">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="990d8-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="990d8-171">例</span><span class="sxs-lookup"><span data-stu-id="990d8-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="990d8-172">要求</span><span class="sxs-lookup"><span data-stu-id="990d8-172">Request</span></span>
<span data-ttu-id="990d8-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="990d8-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="990d8-174">応答</span><span class="sxs-lookup"><span data-stu-id="990d8-174">Response</span></span>
<span data-ttu-id="990d8-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="990d8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

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
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



