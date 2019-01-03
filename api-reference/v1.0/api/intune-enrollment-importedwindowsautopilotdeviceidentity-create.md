---
title: Create importedWindowsAutopilotDeviceIdentity
description: 新規で importedWindowsAutopilotDeviceIdentity オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 10dbaed9d10a0b37df9e229d501bb6e469847ea5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334294"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="dc881-103">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="dc881-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="dc881-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc881-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc881-105">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dc881-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc881-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="dc881-106">Prerequisites</span></span>
<span data-ttu-id="dc881-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc881-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc881-109">Permission type</span></span>|<span data-ttu-id="dc881-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc881-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc881-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc881-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc881-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc881-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc881-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc881-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc881-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc881-114">Not supported.</span></span>|
|<span data-ttu-id="dc881-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc881-115">Application</span></span>|<span data-ttu-id="dc881-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc881-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc881-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc881-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="dc881-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc881-118">Request headers</span></span>
|<span data-ttu-id="dc881-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc881-119">Header</span></span>|<span data-ttu-id="dc881-120">値</span><span class="sxs-lookup"><span data-stu-id="dc881-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc881-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc881-121">Authorization</span></span>|<span data-ttu-id="dc881-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dc881-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc881-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dc881-123">Accept</span></span>|<span data-ttu-id="dc881-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc881-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc881-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc881-125">Request body</span></span>
<span data-ttu-id="dc881-126">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc881-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="dc881-127">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dc881-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="dc881-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc881-128">Property</span></span>|<span data-ttu-id="dc881-129">種類</span><span class="sxs-lookup"><span data-stu-id="dc881-129">Type</span></span>|<span data-ttu-id="dc881-130">説明</span><span class="sxs-lookup"><span data-stu-id="dc881-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc881-131">ID</span><span class="sxs-lookup"><span data-stu-id="dc881-131">id</span></span>|<span data-ttu-id="dc881-132">String</span><span class="sxs-lookup"><span data-stu-id="dc881-132">String</span></span>|<span data-ttu-id="dc881-133">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="dc881-133">The GUID for the object</span></span>|
|<span data-ttu-id="dc881-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="dc881-134">orderIdentifier</span></span>|<span data-ttu-id="dc881-135">String</span><span class="sxs-lookup"><span data-stu-id="dc881-135">String</span></span>|<span data-ttu-id="dc881-136">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="dc881-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dc881-137">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="dc881-137">serialNumber</span></span>|<span data-ttu-id="dc881-138">String</span><span class="sxs-lookup"><span data-stu-id="dc881-138">String</span></span>|<span data-ttu-id="dc881-139">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="dc881-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dc881-140">productKey</span><span class="sxs-lookup"><span data-stu-id="dc881-140">productKey</span></span>|<span data-ttu-id="dc881-141">String</span><span class="sxs-lookup"><span data-stu-id="dc881-141">String</span></span>|<span data-ttu-id="dc881-142">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="dc881-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dc881-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="dc881-143">hardwareIdentifier</span></span>|<span data-ttu-id="dc881-144">Binary</span><span class="sxs-lookup"><span data-stu-id="dc881-144">Binary</span></span>|<span data-ttu-id="dc881-145">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="dc881-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dc881-146">state</span><span class="sxs-lookup"><span data-stu-id="dc881-146">state</span></span>|[<span data-ttu-id="dc881-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="dc881-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="dc881-148">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="dc881-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="dc881-149">応答</span><span class="sxs-lookup"><span data-stu-id="dc881-149">Response</span></span>
<span data-ttu-id="dc881-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dc881-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc881-151">例</span><span class="sxs-lookup"><span data-stu-id="dc881-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc881-152">要求</span><span class="sxs-lookup"><span data-stu-id="dc881-152">Request</span></span>
<span data-ttu-id="dc881-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc881-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc881-154">応答</span><span class="sxs-lookup"><span data-stu-id="dc881-154">Response</span></span>
<span data-ttu-id="dc881-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc881-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


