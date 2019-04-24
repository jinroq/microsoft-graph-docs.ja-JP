---
title: importedWindowsAutopilotDeviceIdentity の更新
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a8668fa78c5996b2d33af18e7cbd23a03df1200
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459711"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="180d4-103">importedWindowsAutopilotDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="180d4-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="180d4-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="180d4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="180d4-105">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="180d4-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="180d4-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="180d4-106">Prerequisites</span></span>
<span data-ttu-id="180d4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="180d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="180d4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="180d4-109">Permission type</span></span>|<span data-ttu-id="180d4-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="180d4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="180d4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="180d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="180d4-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="180d4-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="180d4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="180d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="180d4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="180d4-114">Not supported.</span></span>|
|<span data-ttu-id="180d4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="180d4-115">Application</span></span>|<span data-ttu-id="180d4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="180d4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="180d4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="180d4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="180d4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="180d4-118">Request headers</span></span>
|<span data-ttu-id="180d4-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="180d4-119">Header</span></span>|<span data-ttu-id="180d4-120">値</span><span class="sxs-lookup"><span data-stu-id="180d4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="180d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="180d4-121">Authorization</span></span>|<span data-ttu-id="180d4-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="180d4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="180d4-123">承諾</span><span class="sxs-lookup"><span data-stu-id="180d4-123">Accept</span></span>|<span data-ttu-id="180d4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="180d4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="180d4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="180d4-125">Request body</span></span>
<span data-ttu-id="180d4-126">要求本文で、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="180d4-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="180d4-127">次の表に、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="180d4-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="180d4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="180d4-128">Property</span></span>|<span data-ttu-id="180d4-129">型</span><span class="sxs-lookup"><span data-stu-id="180d4-129">Type</span></span>|<span data-ttu-id="180d4-130">説明</span><span class="sxs-lookup"><span data-stu-id="180d4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="180d4-131">id</span><span class="sxs-lookup"><span data-stu-id="180d4-131">id</span></span>|<span data-ttu-id="180d4-132">String</span><span class="sxs-lookup"><span data-stu-id="180d4-132">String</span></span>|<span data-ttu-id="180d4-133">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="180d4-133">The GUID for the object</span></span>|
|<span data-ttu-id="180d4-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="180d4-134">orderIdentifier</span></span>|<span data-ttu-id="180d4-135">String</span><span class="sxs-lookup"><span data-stu-id="180d4-135">String</span></span>|<span data-ttu-id="180d4-136">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="180d4-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="180d4-137">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="180d4-137">serialNumber</span></span>|<span data-ttu-id="180d4-138">String</span><span class="sxs-lookup"><span data-stu-id="180d4-138">String</span></span>|<span data-ttu-id="180d4-139">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="180d4-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="180d4-140">productKey</span><span class="sxs-lookup"><span data-stu-id="180d4-140">productKey</span></span>|<span data-ttu-id="180d4-141">String</span><span class="sxs-lookup"><span data-stu-id="180d4-141">String</span></span>|<span data-ttu-id="180d4-142">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="180d4-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="180d4-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="180d4-143">hardwareIdentifier</span></span>|<span data-ttu-id="180d4-144">Binary</span><span class="sxs-lookup"><span data-stu-id="180d4-144">Binary</span></span>|<span data-ttu-id="180d4-145">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="180d4-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="180d4-146">state</span><span class="sxs-lookup"><span data-stu-id="180d4-146">state</span></span>|[<span data-ttu-id="180d4-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="180d4-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="180d4-148">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="180d4-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="180d4-149">応答</span><span class="sxs-lookup"><span data-stu-id="180d4-149">Response</span></span>
<span data-ttu-id="180d4-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="180d4-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="180d4-151">例</span><span class="sxs-lookup"><span data-stu-id="180d4-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="180d4-152">要求</span><span class="sxs-lookup"><span data-stu-id="180d4-152">Request</span></span>
<span data-ttu-id="180d4-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="180d4-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="180d4-154">応答</span><span class="sxs-lookup"><span data-stu-id="180d4-154">Response</span></span>
<span data-ttu-id="180d4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="180d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



