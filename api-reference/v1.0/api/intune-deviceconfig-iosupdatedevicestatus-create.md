---
title: iosUpdateDeviceStatus の作成
description: 新しい iosUpdateDeviceStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7338ddc7937ffb0e6cf1aae6cc20b9f75e720e02
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991252"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="9c5b6-103">iosUpdateDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="9c5b6-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="9c5b6-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c5b6-105">新しい [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-105">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c5b6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9c5b6-106">Prerequisites</span></span>
<span data-ttu-id="9c5b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c5b6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9c5b6-109">Permission type</span></span>|<span data-ttu-id="9c5b6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9c5b6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c5b6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9c5b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c5b6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c5b6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c5b6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9c5b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c5b6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-114">Not supported.</span></span>|
|<span data-ttu-id="9c5b6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9c5b6-115">Application</span></span>|<span data-ttu-id="9c5b6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c5b6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9c5b6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9c5b6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c5b6-118">Request headers</span></span>
|<span data-ttu-id="9c5b6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c5b6-119">Header</span></span>|<span data-ttu-id="9c5b6-120">値</span><span class="sxs-lookup"><span data-stu-id="9c5b6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c5b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c5b6-121">Authorization</span></span>|<span data-ttu-id="9c5b6-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c5b6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9c5b6-123">Accept</span></span>|<span data-ttu-id="9c5b6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9c5b6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c5b6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9c5b6-125">Request body</span></span>
<span data-ttu-id="9c5b6-126">要求本文で、iosUpdateDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-126">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="9c5b6-127">次の表に、iosUpdateDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-127">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="9c5b6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c5b6-128">Property</span></span>|<span data-ttu-id="9c5b6-129">型</span><span class="sxs-lookup"><span data-stu-id="9c5b6-129">Type</span></span>|<span data-ttu-id="9c5b6-130">説明</span><span class="sxs-lookup"><span data-stu-id="9c5b6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c5b6-131">ID</span><span class="sxs-lookup"><span data-stu-id="9c5b6-131">id</span></span>|<span data-ttu-id="9c5b6-132">String</span><span class="sxs-lookup"><span data-stu-id="9c5b6-132">String</span></span>|<span data-ttu-id="9c5b6-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-133">Key of the entity.</span></span>|
|<span data-ttu-id="9c5b6-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="9c5b6-134">installStatus</span></span>|[<span data-ttu-id="9c5b6-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9c5b6-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="9c5b6-136">ポリシー レポートのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-136">The installation status of the policy report.</span></span> <span data-ttu-id="9c5b6-137">使用可能な値: `success`、 `available`、 `idle`、 `unknown`、 `downloading`、 `downloadFailed`、 `downloadRequiresComputer`、 `downloadInsufficientSpace`、 `downloadInsufficientPower`、 `downloadInsufficientNetwork`、 `installing`、 `installInsufficientSpace`、 `installInsufficientPower`、 `installPhoneCallInProgress`、 `installFailed`、 `notSupportedOperation`、 `sharedDeviceUserLoggedInError`。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="9c5b6-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="9c5b6-138">osVersion</span></span>|<span data-ttu-id="9c5b6-139">String</span><span class="sxs-lookup"><span data-stu-id="9c5b6-139">String</span></span>|<span data-ttu-id="9c5b6-140">レポートされているデバイス バージョン。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="9c5b6-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="9c5b6-141">deviceId</span></span>|<span data-ttu-id="9c5b6-142">String</span><span class="sxs-lookup"><span data-stu-id="9c5b6-142">String</span></span>|<span data-ttu-id="9c5b6-143">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="9c5b6-144">userId</span><span class="sxs-lookup"><span data-stu-id="9c5b6-144">userId</span></span>|<span data-ttu-id="9c5b6-145">String</span><span class="sxs-lookup"><span data-stu-id="9c5b6-145">String</span></span>|<span data-ttu-id="9c5b6-146">レポートされているユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="9c5b6-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9c5b6-147">deviceDisplayName</span></span>|<span data-ttu-id="9c5b6-148">String</span><span class="sxs-lookup"><span data-stu-id="9c5b6-148">String</span></span>|<span data-ttu-id="9c5b6-149">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="9c5b6-150">userName</span><span class="sxs-lookup"><span data-stu-id="9c5b6-150">userName</span></span>|<span data-ttu-id="9c5b6-151">String</span><span class="sxs-lookup"><span data-stu-id="9c5b6-151">String</span></span>|<span data-ttu-id="9c5b6-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="9c5b6-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="9c5b6-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9c5b6-153">deviceModel</span></span>|<span data-ttu-id="9c5b6-154">String</span><span class="sxs-lookup"><span data-stu-id="9c5b6-154">String</span></span>|<span data-ttu-id="9c5b6-155">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="9c5b6-155">The device model that is being reported</span></span>|
|<span data-ttu-id="9c5b6-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9c5b6-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9c5b6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c5b6-157">DateTimeOffset</span></span>|<span data-ttu-id="9c5b6-158">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="9c5b6-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="9c5b6-159">status</span><span class="sxs-lookup"><span data-stu-id="9c5b6-159">status</span></span>|[<span data-ttu-id="9c5b6-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9c5b6-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9c5b6-161">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-161">Compliance status of the policy report.</span></span> <span data-ttu-id="9c5b6-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9c5b6-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c5b6-163">lastReportedDateTime</span></span>|<span data-ttu-id="9c5b6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c5b6-164">DateTimeOffset</span></span>|<span data-ttu-id="9c5b6-165">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="9c5b6-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c5b6-166">userPrincipalName</span></span>|<span data-ttu-id="9c5b6-167">String</span><span class="sxs-lookup"><span data-stu-id="9c5b6-167">String</span></span>|<span data-ttu-id="9c5b6-168">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="9c5b6-169">応答</span><span class="sxs-lookup"><span data-stu-id="9c5b6-169">Response</span></span>
<span data-ttu-id="9c5b6-170">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-170">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c5b6-171">例</span><span class="sxs-lookup"><span data-stu-id="9c5b6-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c5b6-172">要求</span><span class="sxs-lookup"><span data-stu-id="9c5b6-172">Request</span></span>
<span data-ttu-id="9c5b6-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
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

### <a name="response"></a><span data-ttu-id="9c5b6-174">応答</span><span class="sxs-lookup"><span data-stu-id="9c5b6-174">Response</span></span>
<span data-ttu-id="9c5b6-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9c5b6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



