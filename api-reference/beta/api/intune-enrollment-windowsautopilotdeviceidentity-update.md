---
title: windowsAutopilotDeviceIdentity の更新
description: windowsAutopilotDeviceIdentity オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4132ebc9d93eae71712b04479c1139e1942a9979
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958733"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="bebf8-103">windowsAutopilotDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="bebf8-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="bebf8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bebf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bebf8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bebf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bebf8-106">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bebf8-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bebf8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bebf8-107">Prerequisites</span></span>
<span data-ttu-id="bebf8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bebf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bebf8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bebf8-110">Permission type</span></span>|<span data-ttu-id="bebf8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bebf8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bebf8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bebf8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bebf8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bebf8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bebf8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bebf8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bebf8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bebf8-115">Not supported.</span></span>|
|<span data-ttu-id="bebf8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bebf8-116">Application</span></span>|<span data-ttu-id="bebf8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bebf8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bebf8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bebf8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="bebf8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bebf8-119">Request headers</span></span>
|<span data-ttu-id="bebf8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bebf8-120">Header</span></span>|<span data-ttu-id="bebf8-121">値</span><span class="sxs-lookup"><span data-stu-id="bebf8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bebf8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bebf8-122">Authorization</span></span>|<span data-ttu-id="bebf8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bebf8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bebf8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bebf8-124">Accept</span></span>|<span data-ttu-id="bebf8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bebf8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bebf8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bebf8-126">Request body</span></span>
<span data-ttu-id="bebf8-127">要求本文で、 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bebf8-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="bebf8-128">次の表に、 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bebf8-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="bebf8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bebf8-129">Property</span></span>|<span data-ttu-id="bebf8-130">型</span><span class="sxs-lookup"><span data-stu-id="bebf8-130">Type</span></span>|<span data-ttu-id="bebf8-131">説明</span><span class="sxs-lookup"><span data-stu-id="bebf8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bebf8-132">id</span><span class="sxs-lookup"><span data-stu-id="bebf8-132">id</span></span>|<span data-ttu-id="bebf8-133">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-133">String</span></span>|<span data-ttu-id="bebf8-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="bebf8-134">The GUID for the object</span></span>|
|<span data-ttu-id="bebf8-135">deploymentprofileの状態</span><span class="sxs-lookup"><span data-stu-id="bebf8-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="bebf8-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="bebf8-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="bebf8-137">Windows 自動操縦デバイスのプロファイル割り当て状態。</span><span class="sxs-lookup"><span data-stu-id="bebf8-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="bebf8-138">可能な値は、`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="bebf8-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="bebf8-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="bebf8-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="bebf8-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="bebf8-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="bebf8-141">プロファイルの割り当て Windows 自動操縦デバイスの詳細な状態。</span><span class="sxs-lookup"><span data-stu-id="bebf8-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="bebf8-142">可能な値は、`none`、`hardwareRequirementsNotMet` です。</span><span class="sxs-lookup"><span data-stu-id="bebf8-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="bebf8-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="bebf8-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="bebf8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bebf8-144">DateTimeOffset</span></span>|<span data-ttu-id="bebf8-145">プロファイル Windows 自動操縦デバイスの時間を設定します。</span><span class="sxs-lookup"><span data-stu-id="bebf8-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="bebf8-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="bebf8-146">orderIdentifier</span></span>|<span data-ttu-id="bebf8-147">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-147">String</span></span>|<span data-ttu-id="bebf8-148">Windows 自動操縦デバイスの注文識別子です。</span><span class="sxs-lookup"><span data-stu-id="bebf8-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="bebf8-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="bebf8-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="bebf8-150">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-150">String</span></span>|<span data-ttu-id="bebf8-151">Windows 自動操縦デバイスの注文 id。</span><span class="sxs-lookup"><span data-stu-id="bebf8-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="bebf8-152">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="bebf8-152">serialNumber</span></span>|<span data-ttu-id="bebf8-153">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-153">String</span></span>|<span data-ttu-id="bebf8-154">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="bebf8-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="bebf8-155">productKey</span><span class="sxs-lookup"><span data-stu-id="bebf8-155">productKey</span></span>|<span data-ttu-id="bebf8-156">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-156">String</span></span>|<span data-ttu-id="bebf8-157">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="bebf8-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="bebf8-158">manufacturer</span><span class="sxs-lookup"><span data-stu-id="bebf8-158">manufacturer</span></span>|<span data-ttu-id="bebf8-159">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-159">String</span></span>|<span data-ttu-id="bebf8-160">Windows 自動操縦デバイスの Oem メーカー。</span><span class="sxs-lookup"><span data-stu-id="bebf8-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="bebf8-161">model</span><span class="sxs-lookup"><span data-stu-id="bebf8-161">model</span></span>|<span data-ttu-id="bebf8-162">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-162">String</span></span>|<span data-ttu-id="bebf8-163">Windows 自動操縦デバイスのモデル名です。</span><span class="sxs-lookup"><span data-stu-id="bebf8-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="bebf8-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="bebf8-164">enrollmentState</span></span>|[<span data-ttu-id="bebf8-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="bebf8-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="bebf8-166">Windows 自動操縦デバイスの Intune 登録状態。</span><span class="sxs-lookup"><span data-stu-id="bebf8-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="bebf8-167">可能な値は `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="bebf8-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="bebf8-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="bebf8-168">lastContactedDateTime</span></span>|<span data-ttu-id="bebf8-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bebf8-169">DateTimeOffset</span></span>|<span data-ttu-id="bebf8-170">Intune 前回の接続 Windows 自動操縦デバイスの日時。</span><span class="sxs-lookup"><span data-stu-id="bebf8-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="bebf8-171">addressableusername</span><span class="sxs-lookup"><span data-stu-id="bebf8-171">addressableUserName</span></span>|<span data-ttu-id="bebf8-172">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-172">String</span></span>|<span data-ttu-id="bebf8-173">アドレス指定可能なユーザー名。</span><span class="sxs-lookup"><span data-stu-id="bebf8-173">Addressable user name.</span></span>|
|<span data-ttu-id="bebf8-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bebf8-174">userPrincipalName</span></span>|<span data-ttu-id="bebf8-175">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-175">String</span></span>|<span data-ttu-id="bebf8-176">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="bebf8-176">User Principal Name.</span></span>|
|<span data-ttu-id="bebf8-177">resourceName</span><span class="sxs-lookup"><span data-stu-id="bebf8-177">resourceName</span></span>|<span data-ttu-id="bebf8-178">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-178">String</span></span>|<span data-ttu-id="bebf8-179">リソース名。</span><span class="sxs-lookup"><span data-stu-id="bebf8-179">Resource Name.</span></span>|
|<span data-ttu-id="bebf8-180">skuNumber</span><span class="sxs-lookup"><span data-stu-id="bebf8-180">skuNumber</span></span>|<span data-ttu-id="bebf8-181">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-181">String</span></span>|<span data-ttu-id="bebf8-182">SKU 番号</span><span class="sxs-lookup"><span data-stu-id="bebf8-182">SKU Number</span></span>|
|<span data-ttu-id="bebf8-183">systemfamily</span><span class="sxs-lookup"><span data-stu-id="bebf8-183">systemFamily</span></span>|<span data-ttu-id="bebf8-184">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-184">String</span></span>|<span data-ttu-id="bebf8-185">システムファミリ</span><span class="sxs-lookup"><span data-stu-id="bebf8-185">System Family</span></span>|
|<span data-ttu-id="bebf8-186">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="bebf8-186">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="bebf8-187">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-187">String</span></span>|<span data-ttu-id="bebf8-188">AAD デバイス ID</span><span class="sxs-lookup"><span data-stu-id="bebf8-188">AAD Device ID</span></span>|
|<span data-ttu-id="bebf8-189">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="bebf8-189">managedDeviceId</span></span>|<span data-ttu-id="bebf8-190">String</span><span class="sxs-lookup"><span data-stu-id="bebf8-190">String</span></span>|<span data-ttu-id="bebf8-191">管理対象デバイス ID</span><span class="sxs-lookup"><span data-stu-id="bebf8-191">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="bebf8-192">応答</span><span class="sxs-lookup"><span data-stu-id="bebf8-192">Response</span></span>
<span data-ttu-id="bebf8-193">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bebf8-193">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bebf8-194">例</span><span class="sxs-lookup"><span data-stu-id="bebf8-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="bebf8-195">要求</span><span class="sxs-lookup"><span data-stu-id="bebf8-195">Request</span></span>
<span data-ttu-id="bebf8-196">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bebf8-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 1001

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="bebf8-197">応答</span><span class="sxs-lookup"><span data-stu-id="bebf8-197">Response</span></span>
<span data-ttu-id="bebf8-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bebf8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1050

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value"
}
```




