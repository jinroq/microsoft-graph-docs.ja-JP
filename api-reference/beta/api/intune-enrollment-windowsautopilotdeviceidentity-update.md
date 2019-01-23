---
title: WindowsAutopilotDeviceIdentity を更新します。
description: WindowsAutopilotDeviceIdentity オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 018b45712ce7a35d2b7a19a09bca7ea7dd1650d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423868"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="ed7ca-103">WindowsAutopilotDeviceIdentity を更新します。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="ed7ca-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ed7ca-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed7ca-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed7ca-107">[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-107">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed7ca-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ed7ca-108">Prerequisites</span></span>
<span data-ttu-id="ed7ca-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ed7ca-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed7ca-111">Permission type</span></span>|<span data-ttu-id="ed7ca-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed7ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed7ca-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed7ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed7ca-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed7ca-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed7ca-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed7ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed7ca-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-116">Not supported.</span></span>|
|<span data-ttu-id="ed7ca-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed7ca-117">Application</span></span>|<span data-ttu-id="ed7ca-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed7ca-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed7ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="ed7ca-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed7ca-120">Request headers</span></span>
|<span data-ttu-id="ed7ca-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed7ca-121">Header</span></span>|<span data-ttu-id="ed7ca-122">値</span><span class="sxs-lookup"><span data-stu-id="ed7ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed7ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed7ca-123">Authorization</span></span>|<span data-ttu-id="ed7ca-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed7ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed7ca-125">Accept</span></span>|<span data-ttu-id="ed7ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed7ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed7ca-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed7ca-127">Request body</span></span>
<span data-ttu-id="ed7ca-128">要求の本文に[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-128">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="ed7ca-129">[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-129">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="ed7ca-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed7ca-130">Property</span></span>|<span data-ttu-id="ed7ca-131">型</span><span class="sxs-lookup"><span data-stu-id="ed7ca-131">Type</span></span>|<span data-ttu-id="ed7ca-132">説明</span><span class="sxs-lookup"><span data-stu-id="ed7ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed7ca-133">id</span><span class="sxs-lookup"><span data-stu-id="ed7ca-133">id</span></span>|<span data-ttu-id="ed7ca-134">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-134">String</span></span>|<span data-ttu-id="ed7ca-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="ed7ca-135">The GUID for the object</span></span>|
|<span data-ttu-id="ed7ca-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="ed7ca-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="ed7ca-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="ed7ca-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="ed7ca-138">Windows の自動操縦装置のデバイスの割り当ての状態をプロファイルします。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="ed7ca-139">可能な値は、`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="ed7ca-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="ed7ca-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="ed7ca-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="ed7ca-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="ed7ca-142">プロファイルの割り当ては、Windows の自動操縦装置のデバイスの状態を詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="ed7ca-143">使用可能な値は、`none`、`hardwareRequirementsNotMet` です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="ed7ca-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed7ca-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="ed7ca-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed7ca-145">DateTimeOffset</span></span>|<span data-ttu-id="ed7ca-146">プロファイルは、Windows の自動操縦装置のデバイスの時刻を設定します。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ed7ca-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed7ca-147">orderIdentifier</span></span>|<span data-ttu-id="ed7ca-148">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-148">String</span></span>|<span data-ttu-id="ed7ca-149">Windows の自動操縦装置のデバイスの順序の識別子です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ed7ca-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed7ca-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="ed7ca-151">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-151">String</span></span>|<span data-ttu-id="ed7ca-152">Windows の自動操縦装置のデバイスの購買注文の識別子です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ed7ca-153">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="ed7ca-153">serialNumber</span></span>|<span data-ttu-id="ed7ca-154">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-154">String</span></span>|<span data-ttu-id="ed7ca-155">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ed7ca-156">productKey</span><span class="sxs-lookup"><span data-stu-id="ed7ca-156">productKey</span></span>|<span data-ttu-id="ed7ca-157">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-157">String</span></span>|<span data-ttu-id="ed7ca-158">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ed7ca-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ed7ca-159">manufacturer</span></span>|<span data-ttu-id="ed7ca-160">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-160">String</span></span>|<span data-ttu-id="ed7ca-161">Windows の自動操縦装置のデバイスの Oem メーカーです。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ed7ca-162">model</span><span class="sxs-lookup"><span data-stu-id="ed7ca-162">model</span></span>|<span data-ttu-id="ed7ca-163">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-163">String</span></span>|<span data-ttu-id="ed7ca-164">Windows の自動操縦装置のデバイスのモデル名です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ed7ca-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ed7ca-165">enrollmentState</span></span>|[<span data-ttu-id="ed7ca-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ed7ca-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="ed7ca-167">Intune Windows の自動操縦装置のデバイスの状態を登録します。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="ed7ca-168">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ed7ca-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed7ca-169">lastContactedDateTime</span></span>|<span data-ttu-id="ed7ca-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed7ca-170">DateTimeOffset</span></span>|<span data-ttu-id="ed7ca-171">Intune 最終接続日時 Windows の自動操縦装置のデバイスのです。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ed7ca-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="ed7ca-172">addressableUserName</span></span>|<span data-ttu-id="ed7ca-173">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-173">String</span></span>|<span data-ttu-id="ed7ca-174">アドレス指定可能なユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-174">Addressable user name.</span></span>|
|<span data-ttu-id="ed7ca-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed7ca-175">userPrincipalName</span></span>|<span data-ttu-id="ed7ca-176">String</span><span class="sxs-lookup"><span data-stu-id="ed7ca-176">String</span></span>|<span data-ttu-id="ed7ca-177">ユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="ed7ca-178">応答</span><span class="sxs-lookup"><span data-stu-id="ed7ca-178">Response</span></span>
<span data-ttu-id="ed7ca-179">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-179">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed7ca-180">例</span><span class="sxs-lookup"><span data-stu-id="ed7ca-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed7ca-181">要求</span><span class="sxs-lookup"><span data-stu-id="ed7ca-181">Request</span></span>
<span data-ttu-id="ed7ca-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="ed7ca-183">応答</span><span class="sxs-lookup"><span data-stu-id="ed7ca-183">Response</span></span>
<span data-ttu-id="ed7ca-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed7ca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




