---
title: WindowsAutopilotDeviceIdentity を作成します。
description: 新しい windowsAutopilotDeviceIdentity オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 1e4a9d43755fff787efa08a8c727e6ddc35fa904
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316017"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="c860a-103">WindowsAutopilotDeviceIdentity を作成します。</span><span class="sxs-lookup"><span data-stu-id="c860a-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="c860a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c860a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c860a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c860a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c860a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c860a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c860a-107">新しい[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c860a-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c860a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c860a-108">Prerequisites</span></span>
<span data-ttu-id="c860a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c860a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c860a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c860a-111">Permission type</span></span>|<span data-ttu-id="c860a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c860a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c860a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c860a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c860a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c860a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c860a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c860a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c860a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c860a-116">Not supported.</span></span>|
|<span data-ttu-id="c860a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c860a-117">Application</span></span>|<span data-ttu-id="c860a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c860a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c860a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c860a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="c860a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c860a-120">Request headers</span></span>
|<span data-ttu-id="c860a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c860a-121">Header</span></span>|<span data-ttu-id="c860a-122">値</span><span class="sxs-lookup"><span data-stu-id="c860a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c860a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c860a-123">Authorization</span></span>|<span data-ttu-id="c860a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c860a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c860a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c860a-125">Accept</span></span>|<span data-ttu-id="c860a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c860a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c860a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c860a-127">Request body</span></span>
<span data-ttu-id="c860a-128">要求の本文に windowsAutopilotDeviceIdentity オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c860a-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="c860a-129">次の表は、windowsAutopilotDeviceIdentity を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c860a-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="c860a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c860a-130">Property</span></span>|<span data-ttu-id="c860a-131">種類</span><span class="sxs-lookup"><span data-stu-id="c860a-131">Type</span></span>|<span data-ttu-id="c860a-132">説明</span><span class="sxs-lookup"><span data-stu-id="c860a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c860a-133">ID</span><span class="sxs-lookup"><span data-stu-id="c860a-133">id</span></span>|<span data-ttu-id="c860a-134">String</span><span class="sxs-lookup"><span data-stu-id="c860a-134">String</span></span>|<span data-ttu-id="c860a-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="c860a-135">The GUID for the object</span></span>|
|<span data-ttu-id="c860a-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="c860a-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="c860a-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="c860a-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="c860a-138">Windows の自動操縦装置のデバイスの割り当ての状態をプロファイルします。</span><span class="sxs-lookup"><span data-stu-id="c860a-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="c860a-139">可能な値は、`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="c860a-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="c860a-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="c860a-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="c860a-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="c860a-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="c860a-142">プロファイルの割り当ては、Windows の自動操縦装置のデバイスの状態を詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="c860a-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="c860a-143">使用可能な値は、`none`、`hardwareRequirementsNotMet` です。</span><span class="sxs-lookup"><span data-stu-id="c860a-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="c860a-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="c860a-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="c860a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c860a-145">DateTimeOffset</span></span>|<span data-ttu-id="c860a-146">プロファイルは、Windows の自動操縦装置のデバイスの時刻を設定します。</span><span class="sxs-lookup"><span data-stu-id="c860a-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c860a-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="c860a-147">orderIdentifier</span></span>|<span data-ttu-id="c860a-148">String</span><span class="sxs-lookup"><span data-stu-id="c860a-148">String</span></span>|<span data-ttu-id="c860a-149">Windows の自動操縦装置のデバイスの順序の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c860a-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c860a-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="c860a-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="c860a-151">String</span><span class="sxs-lookup"><span data-stu-id="c860a-151">String</span></span>|<span data-ttu-id="c860a-152">Windows の自動操縦装置のデバイスの購買注文の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c860a-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c860a-153">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="c860a-153">serialNumber</span></span>|<span data-ttu-id="c860a-154">String</span><span class="sxs-lookup"><span data-stu-id="c860a-154">String</span></span>|<span data-ttu-id="c860a-155">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="c860a-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c860a-156">productKey</span><span class="sxs-lookup"><span data-stu-id="c860a-156">productKey</span></span>|<span data-ttu-id="c860a-157">String</span><span class="sxs-lookup"><span data-stu-id="c860a-157">String</span></span>|<span data-ttu-id="c860a-158">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="c860a-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c860a-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="c860a-159">manufacturer</span></span>|<span data-ttu-id="c860a-160">String</span><span class="sxs-lookup"><span data-stu-id="c860a-160">String</span></span>|<span data-ttu-id="c860a-161">Windows の自動操縦装置のデバイスの Oem メーカーです。</span><span class="sxs-lookup"><span data-stu-id="c860a-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c860a-162">model</span><span class="sxs-lookup"><span data-stu-id="c860a-162">model</span></span>|<span data-ttu-id="c860a-163">String</span><span class="sxs-lookup"><span data-stu-id="c860a-163">String</span></span>|<span data-ttu-id="c860a-164">Windows の自動操縦装置のデバイスのモデル名です。</span><span class="sxs-lookup"><span data-stu-id="c860a-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c860a-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c860a-165">enrollmentState</span></span>|[<span data-ttu-id="c860a-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c860a-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="c860a-167">Intune Windows の自動操縦装置のデバイスの状態を登録します。</span><span class="sxs-lookup"><span data-stu-id="c860a-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="c860a-168">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c860a-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c860a-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="c860a-169">lastContactedDateTime</span></span>|<span data-ttu-id="c860a-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c860a-170">DateTimeOffset</span></span>|<span data-ttu-id="c860a-171">Intune 最終接続日時 Windows の自動操縦装置のデバイスのです。</span><span class="sxs-lookup"><span data-stu-id="c860a-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c860a-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="c860a-172">addressableUserName</span></span>|<span data-ttu-id="c860a-173">String</span><span class="sxs-lookup"><span data-stu-id="c860a-173">String</span></span>|<span data-ttu-id="c860a-174">アドレス指定可能なユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="c860a-174">Addressable user name.</span></span>|
|<span data-ttu-id="c860a-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c860a-175">userPrincipalName</span></span>|<span data-ttu-id="c860a-176">String</span><span class="sxs-lookup"><span data-stu-id="c860a-176">String</span></span>|<span data-ttu-id="c860a-177">ユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="c860a-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="c860a-178">応答</span><span class="sxs-lookup"><span data-stu-id="c860a-178">Response</span></span>
<span data-ttu-id="c860a-179">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c860a-179">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c860a-180">例</span><span class="sxs-lookup"><span data-stu-id="c860a-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="c860a-181">要求</span><span class="sxs-lookup"><span data-stu-id="c860a-181">Request</span></span>
<span data-ttu-id="c860a-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c860a-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 755

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
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="c860a-183">応答</span><span class="sxs-lookup"><span data-stu-id="c860a-183">Response</span></span>
<span data-ttu-id="c860a-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c860a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 804

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
  "userPrincipalName": "User Principal Name value"
}
```





