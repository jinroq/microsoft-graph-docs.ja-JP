---
title: iosUpdateDeviceStatus の更新
description: iosUpdateDeviceStatus オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffcaf40ccb95322f84038ed734985048ff0e0aa0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977122"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="744c0-103">iosUpdateDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="744c0-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="744c0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="744c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="744c0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="744c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="744c0-106">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="744c0-106">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="744c0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="744c0-107">Prerequisites</span></span>
<span data-ttu-id="744c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="744c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="744c0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="744c0-110">Permission type</span></span>|<span data-ttu-id="744c0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="744c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="744c0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="744c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="744c0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="744c0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="744c0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="744c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="744c0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="744c0-115">Not supported.</span></span>|
|<span data-ttu-id="744c0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="744c0-116">Application</span></span>|<span data-ttu-id="744c0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="744c0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="744c0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="744c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="744c0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="744c0-119">Request headers</span></span>
|<span data-ttu-id="744c0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="744c0-120">Header</span></span>|<span data-ttu-id="744c0-121">値</span><span class="sxs-lookup"><span data-stu-id="744c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="744c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="744c0-122">Authorization</span></span>|<span data-ttu-id="744c0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="744c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="744c0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="744c0-124">Accept</span></span>|<span data-ttu-id="744c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="744c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="744c0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="744c0-126">Request body</span></span>
<span data-ttu-id="744c0-127">要求本文で、[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="744c0-127">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="744c0-128">次の表に、[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="744c0-128">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="744c0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="744c0-129">Property</span></span>|<span data-ttu-id="744c0-130">型</span><span class="sxs-lookup"><span data-stu-id="744c0-130">Type</span></span>|<span data-ttu-id="744c0-131">説明</span><span class="sxs-lookup"><span data-stu-id="744c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="744c0-132">id</span><span class="sxs-lookup"><span data-stu-id="744c0-132">id</span></span>|<span data-ttu-id="744c0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="744c0-133">String</span></span>|<span data-ttu-id="744c0-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="744c0-134">Key of the entity.</span></span>|
|<span data-ttu-id="744c0-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="744c0-135">installStatus</span></span>|[<span data-ttu-id="744c0-136">Iosupの Installstatus</span><span class="sxs-lookup"><span data-stu-id="744c0-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="744c0-137">ポリシー レポートのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="744c0-137">The installation status of the policy report.</span></span> <span data-ttu-id="744c0-138">可能な値は`success`、 `available`、 `idle` `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `sharedDeviceUserLoggedInError`、、 `installing`、、、、、、、、です。 `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation`</span><span class="sxs-lookup"><span data-stu-id="744c0-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="744c0-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="744c0-139">osVersion</span></span>|<span data-ttu-id="744c0-140">String</span><span class="sxs-lookup"><span data-stu-id="744c0-140">String</span></span>|<span data-ttu-id="744c0-141">レポートされているデバイス バージョン。</span><span class="sxs-lookup"><span data-stu-id="744c0-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="744c0-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="744c0-142">deviceId</span></span>|<span data-ttu-id="744c0-143">String</span><span class="sxs-lookup"><span data-stu-id="744c0-143">String</span></span>|<span data-ttu-id="744c0-144">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="744c0-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="744c0-145">userId</span><span class="sxs-lookup"><span data-stu-id="744c0-145">userId</span></span>|<span data-ttu-id="744c0-146">String</span><span class="sxs-lookup"><span data-stu-id="744c0-146">String</span></span>|<span data-ttu-id="744c0-147">レポートされているユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="744c0-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="744c0-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="744c0-148">deviceDisplayName</span></span>|<span data-ttu-id="744c0-149">String</span><span class="sxs-lookup"><span data-stu-id="744c0-149">String</span></span>|<span data-ttu-id="744c0-150">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="744c0-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="744c0-151">userName</span><span class="sxs-lookup"><span data-stu-id="744c0-151">userName</span></span>|<span data-ttu-id="744c0-152">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="744c0-152">String</span></span>|<span data-ttu-id="744c0-153">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="744c0-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="744c0-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="744c0-154">deviceModel</span></span>|<span data-ttu-id="744c0-155">String</span><span class="sxs-lookup"><span data-stu-id="744c0-155">String</span></span>|<span data-ttu-id="744c0-156">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="744c0-156">The device model that is being reported</span></span>|
|<span data-ttu-id="744c0-157">platform</span><span class="sxs-lookup"><span data-stu-id="744c0-157">platform</span></span>|<span data-ttu-id="744c0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="744c0-158">Int32</span></span>|<span data-ttu-id="744c0-159">レポートされているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="744c0-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="744c0-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="744c0-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="744c0-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="744c0-161">DateTimeOffset</span></span>|<span data-ttu-id="744c0-162">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="744c0-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="744c0-163">status</span><span class="sxs-lookup"><span data-stu-id="744c0-163">status</span></span>|[<span data-ttu-id="744c0-164">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="744c0-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="744c0-165">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="744c0-165">Compliance status of the policy report.</span></span> <span data-ttu-id="744c0-166">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="744c0-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="744c0-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="744c0-167">lastReportedDateTime</span></span>|<span data-ttu-id="744c0-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="744c0-168">DateTimeOffset</span></span>|<span data-ttu-id="744c0-169">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="744c0-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="744c0-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="744c0-170">userPrincipalName</span></span>|<span data-ttu-id="744c0-171">String</span><span class="sxs-lookup"><span data-stu-id="744c0-171">String</span></span>|<span data-ttu-id="744c0-172">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="744c0-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="744c0-173">応答</span><span class="sxs-lookup"><span data-stu-id="744c0-173">Response</span></span>
<span data-ttu-id="744c0-174">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="744c0-174">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="744c0-175">例</span><span class="sxs-lookup"><span data-stu-id="744c0-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="744c0-176">要求</span><span class="sxs-lookup"><span data-stu-id="744c0-176">Request</span></span>
<span data-ttu-id="744c0-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="744c0-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="744c0-178">応答</span><span class="sxs-lookup"><span data-stu-id="744c0-178">Response</span></span>
<span data-ttu-id="744c0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="744c0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





