---
title: Create importedWindowsAutopilotDeviceIdentity
description: 新規で importedWindowsAutopilotDeviceIdentity オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dcd78ce37bdc4718bb69ed324ab34c12d2c7096
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908421"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="65a15-103">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="65a15-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="65a15-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65a15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65a15-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65a15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65a15-106">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="65a15-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65a15-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="65a15-107">Prerequisites</span></span>
<span data-ttu-id="65a15-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65a15-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65a15-110">Permission type</span></span>|<span data-ttu-id="65a15-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="65a15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65a15-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65a15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65a15-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a15-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="65a15-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65a15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65a15-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65a15-115">Not supported.</span></span>|
|<span data-ttu-id="65a15-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65a15-116">Application</span></span>|<span data-ttu-id="65a15-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65a15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65a15-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65a15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="65a15-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65a15-119">Request headers</span></span>
|<span data-ttu-id="65a15-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65a15-120">Header</span></span>|<span data-ttu-id="65a15-121">値</span><span class="sxs-lookup"><span data-stu-id="65a15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65a15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65a15-122">Authorization</span></span>|<span data-ttu-id="65a15-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="65a15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65a15-124">承諾</span><span class="sxs-lookup"><span data-stu-id="65a15-124">Accept</span></span>|<span data-ttu-id="65a15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65a15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65a15-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="65a15-126">Request body</span></span>
<span data-ttu-id="65a15-127">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="65a15-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="65a15-128">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="65a15-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="65a15-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65a15-129">Property</span></span>|<span data-ttu-id="65a15-130">型</span><span class="sxs-lookup"><span data-stu-id="65a15-130">Type</span></span>|<span data-ttu-id="65a15-131">説明</span><span class="sxs-lookup"><span data-stu-id="65a15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65a15-132">id</span><span class="sxs-lookup"><span data-stu-id="65a15-132">id</span></span>|<span data-ttu-id="65a15-133">String</span><span class="sxs-lookup"><span data-stu-id="65a15-133">String</span></span>|<span data-ttu-id="65a15-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="65a15-134">The GUID for the object</span></span>|
|<span data-ttu-id="65a15-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="65a15-135">orderIdentifier</span></span>|<span data-ttu-id="65a15-136">String</span><span class="sxs-lookup"><span data-stu-id="65a15-136">String</span></span>|<span data-ttu-id="65a15-137">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="65a15-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="65a15-138">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="65a15-138">serialNumber</span></span>|<span data-ttu-id="65a15-139">String</span><span class="sxs-lookup"><span data-stu-id="65a15-139">String</span></span>|<span data-ttu-id="65a15-140">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="65a15-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="65a15-141">productKey</span><span class="sxs-lookup"><span data-stu-id="65a15-141">productKey</span></span>|<span data-ttu-id="65a15-142">String</span><span class="sxs-lookup"><span data-stu-id="65a15-142">String</span></span>|<span data-ttu-id="65a15-143">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="65a15-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="65a15-144">のようにします。</span><span class="sxs-lookup"><span data-stu-id="65a15-144">importId</span></span>|<span data-ttu-id="65a15-145">String</span><span class="sxs-lookup"><span data-stu-id="65a15-145">String</span></span>|<span data-ttu-id="65a15-146">Windows 自動操縦デバイスのインポート Id。</span><span class="sxs-lookup"><span data-stu-id="65a15-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="65a15-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="65a15-147">hardwareIdentifier</span></span>|<span data-ttu-id="65a15-148">Binary</span><span class="sxs-lookup"><span data-stu-id="65a15-148">Binary</span></span>|<span data-ttu-id="65a15-149">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="65a15-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="65a15-150">state</span><span class="sxs-lookup"><span data-stu-id="65a15-150">state</span></span>|[<span data-ttu-id="65a15-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="65a15-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="65a15-152">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="65a15-152">Current state of the imported device.</span></span>|
|<span data-ttu-id="65a15-153">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65a15-153">assignedUserPrincipalName</span></span>|<span data-ttu-id="65a15-154">String</span><span class="sxs-lookup"><span data-stu-id="65a15-154">String</span></span>|<span data-ttu-id="65a15-155">デバイスが割り当てられるユーザーの UPN</span><span class="sxs-lookup"><span data-stu-id="65a15-155">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="65a15-156">応答</span><span class="sxs-lookup"><span data-stu-id="65a15-156">Response</span></span>
<span data-ttu-id="65a15-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65a15-157">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65a15-158">例</span><span class="sxs-lookup"><span data-stu-id="65a15-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="65a15-159">要求</span><span class="sxs-lookup"><span data-stu-id="65a15-159">Request</span></span>
<span data-ttu-id="65a15-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65a15-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "importId": "Import Id value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="65a15-161">応答</span><span class="sxs-lookup"><span data-stu-id="65a15-161">Response</span></span>
<span data-ttu-id="65a15-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65a15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 694

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "importId": "Import Id value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```




