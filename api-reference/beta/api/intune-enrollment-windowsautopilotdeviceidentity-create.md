---
title: windowsAutopilotDeviceIdentity を作成する
description: 新しい windowsAutopilotDeviceIdentity オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1fe0f7195007eaf937b1d6d82b20f1978136559
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805776"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="6837b-103">windowsAutopilotDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="6837b-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="6837b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6837b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6837b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6837b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6837b-106">新しい[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6837b-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6837b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6837b-107">Prerequisites</span></span>
<span data-ttu-id="6837b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6837b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6837b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6837b-110">Permission type</span></span>|<span data-ttu-id="6837b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6837b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6837b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6837b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6837b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6837b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6837b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6837b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6837b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6837b-115">Not supported.</span></span>|
|<span data-ttu-id="6837b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6837b-116">Application</span></span>|<span data-ttu-id="6837b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6837b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6837b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6837b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="6837b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6837b-119">Request headers</span></span>
|<span data-ttu-id="6837b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6837b-120">Header</span></span>|<span data-ttu-id="6837b-121">値</span><span class="sxs-lookup"><span data-stu-id="6837b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6837b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6837b-122">Authorization</span></span>|<span data-ttu-id="6837b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6837b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6837b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6837b-124">Accept</span></span>|<span data-ttu-id="6837b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6837b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6837b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6837b-126">Request body</span></span>
<span data-ttu-id="6837b-127">要求本文で、windowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6837b-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="6837b-128">次の表に、windowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6837b-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="6837b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6837b-129">Property</span></span>|<span data-ttu-id="6837b-130">型</span><span class="sxs-lookup"><span data-stu-id="6837b-130">Type</span></span>|<span data-ttu-id="6837b-131">説明</span><span class="sxs-lookup"><span data-stu-id="6837b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6837b-132">id</span><span class="sxs-lookup"><span data-stu-id="6837b-132">id</span></span>|<span data-ttu-id="6837b-133">String</span><span class="sxs-lookup"><span data-stu-id="6837b-133">String</span></span>|<span data-ttu-id="6837b-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="6837b-134">The GUID for the object</span></span>|
|<span data-ttu-id="6837b-135">deploymentprofileの状態</span><span class="sxs-lookup"><span data-stu-id="6837b-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="6837b-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="6837b-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="6837b-137">Windows 自動操縦デバイスのプロファイル割り当て状態。</span><span class="sxs-lookup"><span data-stu-id="6837b-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="6837b-138">可能な値は、`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="6837b-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="6837b-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="6837b-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="6837b-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="6837b-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="6837b-141">プロファイルの割り当て Windows 自動操縦デバイスの詳細な状態。</span><span class="sxs-lookup"><span data-stu-id="6837b-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="6837b-142">可能な値は、`none`、`hardwareRequirementsNotMet` です。</span><span class="sxs-lookup"><span data-stu-id="6837b-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="6837b-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="6837b-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="6837b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6837b-144">DateTimeOffset</span></span>|<span data-ttu-id="6837b-145">プロファイル Windows 自動操縦デバイスの時間を設定します。</span><span class="sxs-lookup"><span data-stu-id="6837b-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6837b-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="6837b-146">orderIdentifier</span></span>|<span data-ttu-id="6837b-147">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-147">String</span></span>|<span data-ttu-id="6837b-148">Windows 自動操縦デバイスの注文識別子-非推奨</span><span class="sxs-lookup"><span data-stu-id="6837b-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="6837b-149">grouptag</span><span class="sxs-lookup"><span data-stu-id="6837b-149">groupTag</span></span>|<span data-ttu-id="6837b-150">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-150">String</span></span>|<span data-ttu-id="6837b-151">Windows 自動操縦デバイスのグループタグ。</span><span class="sxs-lookup"><span data-stu-id="6837b-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6837b-152">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="6837b-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="6837b-153">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-153">String</span></span>|<span data-ttu-id="6837b-154">Windows 自動操縦デバイスの注文 id。</span><span class="sxs-lookup"><span data-stu-id="6837b-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6837b-155">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="6837b-155">serialNumber</span></span>|<span data-ttu-id="6837b-156">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-156">String</span></span>|<span data-ttu-id="6837b-157">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="6837b-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6837b-158">productKey</span><span class="sxs-lookup"><span data-stu-id="6837b-158">productKey</span></span>|<span data-ttu-id="6837b-159">String</span><span class="sxs-lookup"><span data-stu-id="6837b-159">String</span></span>|<span data-ttu-id="6837b-160">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="6837b-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6837b-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="6837b-161">manufacturer</span></span>|<span data-ttu-id="6837b-162">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-162">String</span></span>|<span data-ttu-id="6837b-163">Windows 自動操縦デバイスの Oem メーカー。</span><span class="sxs-lookup"><span data-stu-id="6837b-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6837b-164">model</span><span class="sxs-lookup"><span data-stu-id="6837b-164">model</span></span>|<span data-ttu-id="6837b-165">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-165">String</span></span>|<span data-ttu-id="6837b-166">Windows 自動操縦デバイスのモデル名です。</span><span class="sxs-lookup"><span data-stu-id="6837b-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6837b-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="6837b-167">enrollmentState</span></span>|[<span data-ttu-id="6837b-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="6837b-168">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="6837b-169">Windows 自動操縦デバイスの Intune 登録状態。</span><span class="sxs-lookup"><span data-stu-id="6837b-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="6837b-170">可能な値は `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="6837b-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="6837b-171">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="6837b-171">lastContactedDateTime</span></span>|<span data-ttu-id="6837b-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6837b-172">DateTimeOffset</span></span>|<span data-ttu-id="6837b-173">Intune 前回の接続 Windows 自動操縦デバイスの日時。</span><span class="sxs-lookup"><span data-stu-id="6837b-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="6837b-174">addressableusername</span><span class="sxs-lookup"><span data-stu-id="6837b-174">addressableUserName</span></span>|<span data-ttu-id="6837b-175">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-175">String</span></span>|<span data-ttu-id="6837b-176">アドレス指定可能なユーザー名。</span><span class="sxs-lookup"><span data-stu-id="6837b-176">Addressable user name.</span></span>|
|<span data-ttu-id="6837b-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6837b-177">userPrincipalName</span></span>|<span data-ttu-id="6837b-178">String</span><span class="sxs-lookup"><span data-stu-id="6837b-178">String</span></span>|<span data-ttu-id="6837b-179">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="6837b-179">User Principal Name.</span></span>|
|<span data-ttu-id="6837b-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="6837b-180">resourceName</span></span>|<span data-ttu-id="6837b-181">String</span><span class="sxs-lookup"><span data-stu-id="6837b-181">String</span></span>|<span data-ttu-id="6837b-182">リソース名。</span><span class="sxs-lookup"><span data-stu-id="6837b-182">Resource Name.</span></span>|
|<span data-ttu-id="6837b-183">skuNumber</span><span class="sxs-lookup"><span data-stu-id="6837b-183">skuNumber</span></span>|<span data-ttu-id="6837b-184">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-184">String</span></span>|<span data-ttu-id="6837b-185">SKU 番号</span><span class="sxs-lookup"><span data-stu-id="6837b-185">SKU Number</span></span>|
|<span data-ttu-id="6837b-186">systemfamily</span><span class="sxs-lookup"><span data-stu-id="6837b-186">systemFamily</span></span>|<span data-ttu-id="6837b-187">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-187">String</span></span>|<span data-ttu-id="6837b-188">システムファミリ</span><span class="sxs-lookup"><span data-stu-id="6837b-188">System Family</span></span>|
|<span data-ttu-id="6837b-189">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="6837b-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="6837b-190">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-190">String</span></span>|<span data-ttu-id="6837b-191">AAD デバイス ID</span><span class="sxs-lookup"><span data-stu-id="6837b-191">AAD Device ID</span></span>|
|<span data-ttu-id="6837b-192">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="6837b-192">managedDeviceId</span></span>|<span data-ttu-id="6837b-193">文字列</span><span class="sxs-lookup"><span data-stu-id="6837b-193">String</span></span>|<span data-ttu-id="6837b-194">管理対象デバイス ID</span><span class="sxs-lookup"><span data-stu-id="6837b-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="6837b-195">応答</span><span class="sxs-lookup"><span data-stu-id="6837b-195">Response</span></span>
<span data-ttu-id="6837b-196">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6837b-196">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6837b-197">例</span><span class="sxs-lookup"><span data-stu-id="6837b-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="6837b-198">要求</span><span class="sxs-lookup"><span data-stu-id="6837b-198">Request</span></span>
<span data-ttu-id="6837b-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6837b-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6837b-200">応答</span><span class="sxs-lookup"><span data-stu-id="6837b-200">Response</span></span>
<span data-ttu-id="6837b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6837b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





