---
title: iosUpdateDeviceStatus の作成
description: 新しい iosUpdateDeviceStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f115b542f8fe77a8f6368cd1df7da22f41cb2094
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549833"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="50b95-103">iosUpdateDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="50b95-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="50b95-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50b95-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50b95-105">新しい [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="50b95-105">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50b95-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="50b95-106">Prerequisites</span></span>
<span data-ttu-id="50b95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50b95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b95-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50b95-109">Permission type</span></span>|<span data-ttu-id="50b95-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="50b95-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50b95-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50b95-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50b95-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b95-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50b95-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50b95-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50b95-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50b95-114">Not supported.</span></span>|
|<span data-ttu-id="50b95-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50b95-115">Application</span></span>|<span data-ttu-id="50b95-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50b95-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50b95-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50b95-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="50b95-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50b95-118">Request headers</span></span>
|<span data-ttu-id="50b95-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50b95-119">Header</span></span>|<span data-ttu-id="50b95-120">値</span><span class="sxs-lookup"><span data-stu-id="50b95-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50b95-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50b95-121">Authorization</span></span>|<span data-ttu-id="50b95-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="50b95-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50b95-123">承諾</span><span class="sxs-lookup"><span data-stu-id="50b95-123">Accept</span></span>|<span data-ttu-id="50b95-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50b95-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50b95-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="50b95-125">Request body</span></span>
<span data-ttu-id="50b95-126">要求本文で、iosUpdateDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="50b95-126">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="50b95-127">次の表に、iosUpdateDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="50b95-127">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="50b95-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50b95-128">Property</span></span>|<span data-ttu-id="50b95-129">型</span><span class="sxs-lookup"><span data-stu-id="50b95-129">Type</span></span>|<span data-ttu-id="50b95-130">説明</span><span class="sxs-lookup"><span data-stu-id="50b95-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50b95-131">id</span><span class="sxs-lookup"><span data-stu-id="50b95-131">id</span></span>|<span data-ttu-id="50b95-132">String</span><span class="sxs-lookup"><span data-stu-id="50b95-132">String</span></span>|<span data-ttu-id="50b95-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="50b95-133">Key of the entity.</span></span>|
|<span data-ttu-id="50b95-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="50b95-134">installStatus</span></span>|[<span data-ttu-id="50b95-135">iosupの installstatus</span><span class="sxs-lookup"><span data-stu-id="50b95-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="50b95-136">ポリシー レポートのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="50b95-136">The installation status of the policy report.</span></span> <span data-ttu-id="50b95-137">可能な値は`success`、 `available`、 `idle` `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `sharedDeviceUserLoggedInError`、、 `installing`、、、、、、、、です。 `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation`</span><span class="sxs-lookup"><span data-stu-id="50b95-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="50b95-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="50b95-138">osVersion</span></span>|<span data-ttu-id="50b95-139">String</span><span class="sxs-lookup"><span data-stu-id="50b95-139">String</span></span>|<span data-ttu-id="50b95-140">レポートされているデバイス バージョン。</span><span class="sxs-lookup"><span data-stu-id="50b95-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="50b95-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="50b95-141">deviceId</span></span>|<span data-ttu-id="50b95-142">String</span><span class="sxs-lookup"><span data-stu-id="50b95-142">String</span></span>|<span data-ttu-id="50b95-143">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="50b95-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="50b95-144">userId</span><span class="sxs-lookup"><span data-stu-id="50b95-144">userId</span></span>|<span data-ttu-id="50b95-145">String</span><span class="sxs-lookup"><span data-stu-id="50b95-145">String</span></span>|<span data-ttu-id="50b95-146">レポートされているユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="50b95-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="50b95-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="50b95-147">deviceDisplayName</span></span>|<span data-ttu-id="50b95-148">String</span><span class="sxs-lookup"><span data-stu-id="50b95-148">String</span></span>|<span data-ttu-id="50b95-149">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="50b95-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="50b95-150">userName</span><span class="sxs-lookup"><span data-stu-id="50b95-150">userName</span></span>|<span data-ttu-id="50b95-151">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="50b95-151">String</span></span>|<span data-ttu-id="50b95-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="50b95-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="50b95-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="50b95-153">deviceModel</span></span>|<span data-ttu-id="50b95-154">String</span><span class="sxs-lookup"><span data-stu-id="50b95-154">String</span></span>|<span data-ttu-id="50b95-155">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="50b95-155">The device model that is being reported</span></span>|
|<span data-ttu-id="50b95-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="50b95-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="50b95-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b95-157">DateTimeOffset</span></span>|<span data-ttu-id="50b95-158">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="50b95-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="50b95-159">status</span><span class="sxs-lookup"><span data-stu-id="50b95-159">status</span></span>|[<span data-ttu-id="50b95-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="50b95-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="50b95-161">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="50b95-161">Compliance status of the policy report.</span></span> <span data-ttu-id="50b95-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="50b95-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="50b95-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="50b95-163">lastReportedDateTime</span></span>|<span data-ttu-id="50b95-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50b95-164">DateTimeOffset</span></span>|<span data-ttu-id="50b95-165">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="50b95-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="50b95-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="50b95-166">userPrincipalName</span></span>|<span data-ttu-id="50b95-167">String</span><span class="sxs-lookup"><span data-stu-id="50b95-167">String</span></span>|<span data-ttu-id="50b95-168">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="50b95-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="50b95-169">応答</span><span class="sxs-lookup"><span data-stu-id="50b95-169">Response</span></span>
<span data-ttu-id="50b95-170">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="50b95-170">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b95-171">例</span><span class="sxs-lookup"><span data-stu-id="50b95-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="50b95-172">要求</span><span class="sxs-lookup"><span data-stu-id="50b95-172">Request</span></span>
<span data-ttu-id="50b95-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50b95-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50b95-174">応答</span><span class="sxs-lookup"><span data-stu-id="50b95-174">Response</span></span>
<span data-ttu-id="50b95-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="50b95-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



