---
title: WindowsAutopilotDeviceIdentity を作成する
description: 新しい windowsAutopilotDeviceIdentity オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acc1aa929da940a36bf9c00b5abc5b8c4d5a7d9f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908246"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="fb41e-103">WindowsAutopilotDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="fb41e-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="fb41e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb41e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb41e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fb41e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb41e-106">新しい[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fb41e-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb41e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fb41e-107">Prerequisites</span></span>
<span data-ttu-id="fb41e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb41e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb41e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb41e-110">Permission type</span></span>|<span data-ttu-id="fb41e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb41e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb41e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb41e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb41e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb41e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fb41e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb41e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb41e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb41e-115">Not supported.</span></span>|
|<span data-ttu-id="fb41e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb41e-116">Application</span></span>|<span data-ttu-id="fb41e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb41e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb41e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb41e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="fb41e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb41e-119">Request headers</span></span>
|<span data-ttu-id="fb41e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb41e-120">Header</span></span>|<span data-ttu-id="fb41e-121">値</span><span class="sxs-lookup"><span data-stu-id="fb41e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb41e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb41e-122">Authorization</span></span>|<span data-ttu-id="fb41e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fb41e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb41e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fb41e-124">Accept</span></span>|<span data-ttu-id="fb41e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb41e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb41e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb41e-126">Request body</span></span>
<span data-ttu-id="fb41e-127">要求本文で、windowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb41e-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="fb41e-128">次の表に、windowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fb41e-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="fb41e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb41e-129">Property</span></span>|<span data-ttu-id="fb41e-130">型</span><span class="sxs-lookup"><span data-stu-id="fb41e-130">Type</span></span>|<span data-ttu-id="fb41e-131">説明</span><span class="sxs-lookup"><span data-stu-id="fb41e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb41e-132">id</span><span class="sxs-lookup"><span data-stu-id="fb41e-132">id</span></span>|<span data-ttu-id="fb41e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="fb41e-133">String</span></span>|<span data-ttu-id="fb41e-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="fb41e-134">The GUID for the object</span></span>|
|<span data-ttu-id="fb41e-135">Deploymentprofileの状態</span><span class="sxs-lookup"><span data-stu-id="fb41e-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="fb41e-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="fb41e-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="fb41e-137">Windows 自動操縦デバイスのプロファイル割り当て状態。</span><span class="sxs-lookup"><span data-stu-id="fb41e-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="fb41e-138">可能な値は、`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="fb41e-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="fb41e-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="fb41e-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="fb41e-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="fb41e-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="fb41e-141">プロファイルの割り当て Windows 自動操縦デバイスの詳細な状態。</span><span class="sxs-lookup"><span data-stu-id="fb41e-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="fb41e-142">可能な値は、`none`、`hardwareRequirementsNotMet` です。</span><span class="sxs-lookup"><span data-stu-id="fb41e-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="fb41e-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb41e-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="fb41e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb41e-144">DateTimeOffset</span></span>|<span data-ttu-id="fb41e-145">プロファイル Windows 自動操縦デバイスの時間を設定します。</span><span class="sxs-lookup"><span data-stu-id="fb41e-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fb41e-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="fb41e-146">orderIdentifier</span></span>|<span data-ttu-id="fb41e-147">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-147">String</span></span>|<span data-ttu-id="fb41e-148">Windows 自動操縦デバイスの注文識別子-非推奨</span><span class="sxs-lookup"><span data-stu-id="fb41e-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="fb41e-149">groupTag</span><span class="sxs-lookup"><span data-stu-id="fb41e-149">groupTag</span></span>|<span data-ttu-id="fb41e-150">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-150">String</span></span>|<span data-ttu-id="fb41e-151">Windows 自動操縦デバイスのグループタグ。</span><span class="sxs-lookup"><span data-stu-id="fb41e-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fb41e-152">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="fb41e-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="fb41e-153">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-153">String</span></span>|<span data-ttu-id="fb41e-154">Windows 自動操縦デバイスの注文 Id。</span><span class="sxs-lookup"><span data-stu-id="fb41e-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fb41e-155">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="fb41e-155">serialNumber</span></span>|<span data-ttu-id="fb41e-156">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-156">String</span></span>|<span data-ttu-id="fb41e-157">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="fb41e-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fb41e-158">productKey</span><span class="sxs-lookup"><span data-stu-id="fb41e-158">productKey</span></span>|<span data-ttu-id="fb41e-159">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-159">String</span></span>|<span data-ttu-id="fb41e-160">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="fb41e-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fb41e-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="fb41e-161">manufacturer</span></span>|<span data-ttu-id="fb41e-162">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-162">String</span></span>|<span data-ttu-id="fb41e-163">Windows 自動操縦デバイスの Oem メーカー。</span><span class="sxs-lookup"><span data-stu-id="fb41e-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fb41e-164">model</span><span class="sxs-lookup"><span data-stu-id="fb41e-164">model</span></span>|<span data-ttu-id="fb41e-165">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-165">String</span></span>|<span data-ttu-id="fb41e-166">Windows 自動操縦デバイスのモデル名です。</span><span class="sxs-lookup"><span data-stu-id="fb41e-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fb41e-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="fb41e-167">enrollmentState</span></span>|[<span data-ttu-id="fb41e-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="fb41e-168">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="fb41e-169">Windows 自動操縦デバイスの Intune 登録状態。</span><span class="sxs-lookup"><span data-stu-id="fb41e-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="fb41e-170">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="fb41e-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="fb41e-171">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb41e-171">lastContactedDateTime</span></span>|<span data-ttu-id="fb41e-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb41e-172">DateTimeOffset</span></span>|<span data-ttu-id="fb41e-173">Intune 前回の接続 Windows 自動操縦デバイスの日時。</span><span class="sxs-lookup"><span data-stu-id="fb41e-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fb41e-174">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="fb41e-174">addressableUserName</span></span>|<span data-ttu-id="fb41e-175">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-175">String</span></span>|<span data-ttu-id="fb41e-176">アドレス指定可能なユーザー名。</span><span class="sxs-lookup"><span data-stu-id="fb41e-176">Addressable user name.</span></span>|
|<span data-ttu-id="fb41e-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fb41e-177">userPrincipalName</span></span>|<span data-ttu-id="fb41e-178">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-178">String</span></span>|<span data-ttu-id="fb41e-179">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="fb41e-179">User Principal Name.</span></span>|
|<span data-ttu-id="fb41e-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="fb41e-180">resourceName</span></span>|<span data-ttu-id="fb41e-181">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-181">String</span></span>|<span data-ttu-id="fb41e-182">リソース名。</span><span class="sxs-lookup"><span data-stu-id="fb41e-182">Resource Name.</span></span>|
|<span data-ttu-id="fb41e-183">skuNumber</span><span class="sxs-lookup"><span data-stu-id="fb41e-183">skuNumber</span></span>|<span data-ttu-id="fb41e-184">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-184">String</span></span>|<span data-ttu-id="fb41e-185">SKU 番号</span><span class="sxs-lookup"><span data-stu-id="fb41e-185">SKU Number</span></span>|
|<span data-ttu-id="fb41e-186">systemFamily</span><span class="sxs-lookup"><span data-stu-id="fb41e-186">systemFamily</span></span>|<span data-ttu-id="fb41e-187">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-187">String</span></span>|<span data-ttu-id="fb41e-188">システムファミリ</span><span class="sxs-lookup"><span data-stu-id="fb41e-188">System Family</span></span>|
|<span data-ttu-id="fb41e-189">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="fb41e-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="fb41e-190">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-190">String</span></span>|<span data-ttu-id="fb41e-191">AAD デバイス ID</span><span class="sxs-lookup"><span data-stu-id="fb41e-191">AAD Device ID</span></span>|
|<span data-ttu-id="fb41e-192">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="fb41e-192">managedDeviceId</span></span>|<span data-ttu-id="fb41e-193">String</span><span class="sxs-lookup"><span data-stu-id="fb41e-193">String</span></span>|<span data-ttu-id="fb41e-194">管理対象デバイス ID</span><span class="sxs-lookup"><span data-stu-id="fb41e-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="fb41e-195">応答</span><span class="sxs-lookup"><span data-stu-id="fb41e-195">Response</span></span>
<span data-ttu-id="fb41e-196">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fb41e-196">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb41e-197">例</span><span class="sxs-lookup"><span data-stu-id="fb41e-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb41e-198">要求</span><span class="sxs-lookup"><span data-stu-id="fb41e-198">Request</span></span>
<span data-ttu-id="fb41e-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb41e-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1035

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
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

### <a name="response"></a><span data-ttu-id="fb41e-200">応答</span><span class="sxs-lookup"><span data-stu-id="fb41e-200">Response</span></span>
<span data-ttu-id="fb41e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb41e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1084

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
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




