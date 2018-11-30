---
title: Create importedWindowsAutopilotDeviceIdentity
description: 新規で importedWindowsAutopilotDeviceIdentity オブジェクトを作成します。
ms.openlocfilehash: 3a6923ba43d188ca1cf904285e1f430e1902f595
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022576"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="60cbc-103">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="60cbc-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="60cbc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="60cbc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60cbc-105">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="60cbc-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60cbc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="60cbc-106">Prerequisites</span></span>
<span data-ttu-id="60cbc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60cbc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60cbc-109">Permission type</span></span>|<span data-ttu-id="60cbc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="60cbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60cbc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60cbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60cbc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60cbc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="60cbc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60cbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60cbc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60cbc-114">Not supported.</span></span>|
|<span data-ttu-id="60cbc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60cbc-115">Application</span></span>|<span data-ttu-id="60cbc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60cbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60cbc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60cbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="60cbc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60cbc-118">Request headers</span></span>
|<span data-ttu-id="60cbc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60cbc-119">Header</span></span>|<span data-ttu-id="60cbc-120">値</span><span class="sxs-lookup"><span data-stu-id="60cbc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60cbc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="60cbc-121">Authorization</span></span>|<span data-ttu-id="60cbc-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="60cbc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60cbc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="60cbc-123">Accept</span></span>|<span data-ttu-id="60cbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="60cbc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60cbc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="60cbc-125">Request body</span></span>
<span data-ttu-id="60cbc-126">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="60cbc-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="60cbc-127">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="60cbc-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="60cbc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60cbc-128">Property</span></span>|<span data-ttu-id="60cbc-129">型</span><span class="sxs-lookup"><span data-stu-id="60cbc-129">Type</span></span>|<span data-ttu-id="60cbc-130">説明</span><span class="sxs-lookup"><span data-stu-id="60cbc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60cbc-131">id</span><span class="sxs-lookup"><span data-stu-id="60cbc-131">id</span></span>|<span data-ttu-id="60cbc-132">String</span><span class="sxs-lookup"><span data-stu-id="60cbc-132">String</span></span>|<span data-ttu-id="60cbc-133">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="60cbc-133">The GUID for the object</span></span>|
|<span data-ttu-id="60cbc-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="60cbc-134">orderIdentifier</span></span>|<span data-ttu-id="60cbc-135">String</span><span class="sxs-lookup"><span data-stu-id="60cbc-135">String</span></span>|<span data-ttu-id="60cbc-136">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="60cbc-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="60cbc-137">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="60cbc-137">serialNumber</span></span>|<span data-ttu-id="60cbc-138">String</span><span class="sxs-lookup"><span data-stu-id="60cbc-138">String</span></span>|<span data-ttu-id="60cbc-139">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="60cbc-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="60cbc-140">productKey</span><span class="sxs-lookup"><span data-stu-id="60cbc-140">productKey</span></span>|<span data-ttu-id="60cbc-141">String</span><span class="sxs-lookup"><span data-stu-id="60cbc-141">String</span></span>|<span data-ttu-id="60cbc-142">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="60cbc-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="60cbc-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="60cbc-143">hardwareIdentifier</span></span>|<span data-ttu-id="60cbc-144">バイナリ</span><span class="sxs-lookup"><span data-stu-id="60cbc-144">Binary</span></span>|<span data-ttu-id="60cbc-145">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="60cbc-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="60cbc-146">状態</span><span class="sxs-lookup"><span data-stu-id="60cbc-146">state</span></span>|[<span data-ttu-id="60cbc-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="60cbc-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="60cbc-148">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="60cbc-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="60cbc-149">応答</span><span class="sxs-lookup"><span data-stu-id="60cbc-149">Response</span></span>
<span data-ttu-id="60cbc-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60cbc-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60cbc-151">例</span><span class="sxs-lookup"><span data-stu-id="60cbc-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="60cbc-152">要求</span><span class="sxs-lookup"><span data-stu-id="60cbc-152">Request</span></span>
<span data-ttu-id="60cbc-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60cbc-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a><span data-ttu-id="60cbc-154">応答</span><span class="sxs-lookup"><span data-stu-id="60cbc-154">Response</span></span>
<span data-ttu-id="60cbc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60cbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```


