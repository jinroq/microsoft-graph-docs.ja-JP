---
title: Create importedWindowsAutopilotDeviceIdentity
description: 新規で importedWindowsAutopilotDeviceIdentity オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 664b0d52eea5d61918e234c9fa582fa57f50d8b5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980097"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="d6dfc-103">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d6dfc-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="d6dfc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6dfc-105">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6dfc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d6dfc-106">Prerequisites</span></span>
<span data-ttu-id="d6dfc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6dfc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6dfc-109">Permission type</span></span>|<span data-ttu-id="d6dfc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6dfc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6dfc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6dfc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6dfc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6dfc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d6dfc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6dfc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6dfc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-114">Not supported.</span></span>|
|<span data-ttu-id="d6dfc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6dfc-115">Application</span></span>|<span data-ttu-id="d6dfc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6dfc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6dfc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="d6dfc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6dfc-118">Request headers</span></span>
|<span data-ttu-id="d6dfc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6dfc-119">Header</span></span>|<span data-ttu-id="d6dfc-120">値</span><span class="sxs-lookup"><span data-stu-id="d6dfc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6dfc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6dfc-121">Authorization</span></span>|<span data-ttu-id="d6dfc-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6dfc-123">承諾</span><span class="sxs-lookup"><span data-stu-id="d6dfc-123">Accept</span></span>|<span data-ttu-id="d6dfc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d6dfc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6dfc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6dfc-125">Request body</span></span>
<span data-ttu-id="d6dfc-126">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="d6dfc-127">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="d6dfc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6dfc-128">Property</span></span>|<span data-ttu-id="d6dfc-129">型</span><span class="sxs-lookup"><span data-stu-id="d6dfc-129">Type</span></span>|<span data-ttu-id="d6dfc-130">説明</span><span class="sxs-lookup"><span data-stu-id="d6dfc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6dfc-131">id</span><span class="sxs-lookup"><span data-stu-id="d6dfc-131">id</span></span>|<span data-ttu-id="d6dfc-132">String</span><span class="sxs-lookup"><span data-stu-id="d6dfc-132">String</span></span>|<span data-ttu-id="d6dfc-133">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="d6dfc-133">The GUID for the object</span></span>|
|<span data-ttu-id="d6dfc-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6dfc-134">orderIdentifier</span></span>|<span data-ttu-id="d6dfc-135">String</span><span class="sxs-lookup"><span data-stu-id="d6dfc-135">String</span></span>|<span data-ttu-id="d6dfc-136">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d6dfc-137">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="d6dfc-137">serialNumber</span></span>|<span data-ttu-id="d6dfc-138">String</span><span class="sxs-lookup"><span data-stu-id="d6dfc-138">String</span></span>|<span data-ttu-id="d6dfc-139">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d6dfc-140">productKey</span><span class="sxs-lookup"><span data-stu-id="d6dfc-140">productKey</span></span>|<span data-ttu-id="d6dfc-141">String</span><span class="sxs-lookup"><span data-stu-id="d6dfc-141">String</span></span>|<span data-ttu-id="d6dfc-142">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d6dfc-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6dfc-143">hardwareIdentifier</span></span>|<span data-ttu-id="d6dfc-144">Binary</span><span class="sxs-lookup"><span data-stu-id="d6dfc-144">Binary</span></span>|<span data-ttu-id="d6dfc-145">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d6dfc-146">state</span><span class="sxs-lookup"><span data-stu-id="d6dfc-146">state</span></span>|[<span data-ttu-id="d6dfc-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="d6dfc-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="d6dfc-148">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="d6dfc-149">応答</span><span class="sxs-lookup"><span data-stu-id="d6dfc-149">Response</span></span>
<span data-ttu-id="d6dfc-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6dfc-151">例</span><span class="sxs-lookup"><span data-stu-id="d6dfc-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6dfc-152">要求</span><span class="sxs-lookup"><span data-stu-id="d6dfc-152">Request</span></span>
<span data-ttu-id="d6dfc-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6dfc-154">応答</span><span class="sxs-lookup"><span data-stu-id="d6dfc-154">Response</span></span>
<span data-ttu-id="d6dfc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6dfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



