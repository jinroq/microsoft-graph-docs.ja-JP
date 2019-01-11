---
title: iosUpdateDeviceStatus の更新
description: iosUpdateDeviceStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a7b9d44c13e4432d3b09e72ad91ce1c357778616
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863400"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="84165-103">iosUpdateDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="84165-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="84165-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84165-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84165-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84165-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84165-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="84165-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84165-107">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="84165-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84165-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="84165-108">Prerequisites</span></span>
<span data-ttu-id="84165-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84165-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84165-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84165-111">Permission type</span></span>|<span data-ttu-id="84165-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="84165-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84165-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84165-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84165-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84165-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84165-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84165-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84165-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84165-116">Not supported.</span></span>|
|<span data-ttu-id="84165-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84165-117">Application</span></span>|<span data-ttu-id="84165-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84165-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84165-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84165-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="84165-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84165-120">Request headers</span></span>
|<span data-ttu-id="84165-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84165-121">Header</span></span>|<span data-ttu-id="84165-122">値</span><span class="sxs-lookup"><span data-stu-id="84165-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84165-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84165-123">Authorization</span></span>|<span data-ttu-id="84165-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="84165-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84165-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84165-125">Accept</span></span>|<span data-ttu-id="84165-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84165-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84165-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="84165-127">Request body</span></span>
<span data-ttu-id="84165-128">要求本文で、[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="84165-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="84165-129">次の表に、[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="84165-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="84165-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84165-130">Property</span></span>|<span data-ttu-id="84165-131">種類</span><span class="sxs-lookup"><span data-stu-id="84165-131">Type</span></span>|<span data-ttu-id="84165-132">説明</span><span class="sxs-lookup"><span data-stu-id="84165-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84165-133">ID</span><span class="sxs-lookup"><span data-stu-id="84165-133">id</span></span>|<span data-ttu-id="84165-134">String</span><span class="sxs-lookup"><span data-stu-id="84165-134">String</span></span>|<span data-ttu-id="84165-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="84165-135">Key of the entity.</span></span>|
|<span data-ttu-id="84165-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="84165-136">installStatus</span></span>|[<span data-ttu-id="84165-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="84165-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="84165-138">ポリシー レポートのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="84165-138">The installation status of the policy report.</span></span> <span data-ttu-id="84165-139">使用可能な値: `success`、 `available`、 `idle`、 `unknown`、 `downloading`、 `downloadFailed`、 `downloadRequiresComputer`、 `downloadInsufficientSpace`、 `downloadInsufficientPower`、 `downloadInsufficientNetwork`、 `installing`、 `installInsufficientSpace`、 `installInsufficientPower`、 `installPhoneCallInProgress`、 `installFailed`、 `notSupportedOperation`、 `sharedDeviceUserLoggedInError`。</span><span class="sxs-lookup"><span data-stu-id="84165-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="84165-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="84165-140">osVersion</span></span>|<span data-ttu-id="84165-141">String</span><span class="sxs-lookup"><span data-stu-id="84165-141">String</span></span>|<span data-ttu-id="84165-142">レポートされているデバイス バージョン。</span><span class="sxs-lookup"><span data-stu-id="84165-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="84165-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="84165-143">deviceId</span></span>|<span data-ttu-id="84165-144">String</span><span class="sxs-lookup"><span data-stu-id="84165-144">String</span></span>|<span data-ttu-id="84165-145">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="84165-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="84165-146">userId</span><span class="sxs-lookup"><span data-stu-id="84165-146">userId</span></span>|<span data-ttu-id="84165-147">String</span><span class="sxs-lookup"><span data-stu-id="84165-147">String</span></span>|<span data-ttu-id="84165-148">レポートされているユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="84165-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="84165-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="84165-149">deviceDisplayName</span></span>|<span data-ttu-id="84165-150">String</span><span class="sxs-lookup"><span data-stu-id="84165-150">String</span></span>|<span data-ttu-id="84165-151">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="84165-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="84165-152">userName</span><span class="sxs-lookup"><span data-stu-id="84165-152">userName</span></span>|<span data-ttu-id="84165-153">String</span><span class="sxs-lookup"><span data-stu-id="84165-153">String</span></span>|<span data-ttu-id="84165-154">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="84165-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="84165-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="84165-155">deviceModel</span></span>|<span data-ttu-id="84165-156">String</span><span class="sxs-lookup"><span data-stu-id="84165-156">String</span></span>|<span data-ttu-id="84165-157">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="84165-157">The device model that is being reported</span></span>|
|<span data-ttu-id="84165-158">platform</span><span class="sxs-lookup"><span data-stu-id="84165-158">platform</span></span>|<span data-ttu-id="84165-159">Int32</span><span class="sxs-lookup"><span data-stu-id="84165-159">Int32</span></span>|<span data-ttu-id="84165-160">報告されているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="84165-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="84165-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="84165-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="84165-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84165-162">DateTimeOffset</span></span>|<span data-ttu-id="84165-163">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="84165-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="84165-164">status</span><span class="sxs-lookup"><span data-stu-id="84165-164">status</span></span>|[<span data-ttu-id="84165-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="84165-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="84165-166">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="84165-166">Compliance status of the policy report.</span></span> <span data-ttu-id="84165-167">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="84165-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="84165-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="84165-168">lastReportedDateTime</span></span>|<span data-ttu-id="84165-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84165-169">DateTimeOffset</span></span>|<span data-ttu-id="84165-170">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="84165-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="84165-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84165-171">userPrincipalName</span></span>|<span data-ttu-id="84165-172">String</span><span class="sxs-lookup"><span data-stu-id="84165-172">String</span></span>|<span data-ttu-id="84165-173">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="84165-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="84165-174">応答</span><span class="sxs-lookup"><span data-stu-id="84165-174">Response</span></span>
<span data-ttu-id="84165-175">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="84165-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84165-176">例</span><span class="sxs-lookup"><span data-stu-id="84165-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="84165-177">要求</span><span class="sxs-lookup"><span data-stu-id="84165-177">Request</span></span>
<span data-ttu-id="84165-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="84165-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 510

{
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

### <a name="response"></a><span data-ttu-id="84165-179">応答</span><span class="sxs-lookup"><span data-stu-id="84165-179">Response</span></span>
<span data-ttu-id="84165-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="84165-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





