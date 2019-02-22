---
title: importedWindowsAutopilotDeviceIdentity の更新
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af2e3e113c96f5b91a2c617f1c3d34dd26274bf0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144248"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="96230-103">importedWindowsAutopilotDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="96230-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="96230-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96230-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96230-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96230-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96230-106">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="96230-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96230-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="96230-107">Prerequisites</span></span>
<span data-ttu-id="96230-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="96230-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96230-110">Permission type</span></span>|<span data-ttu-id="96230-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="96230-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96230-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96230-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96230-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96230-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="96230-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96230-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96230-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96230-115">Not supported.</span></span>|
|<span data-ttu-id="96230-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96230-116">Application</span></span>|<span data-ttu-id="96230-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96230-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96230-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96230-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="96230-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96230-119">Request headers</span></span>
|<span data-ttu-id="96230-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96230-120">Header</span></span>|<span data-ttu-id="96230-121">値</span><span class="sxs-lookup"><span data-stu-id="96230-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96230-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96230-122">Authorization</span></span>|<span data-ttu-id="96230-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="96230-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96230-124">承諾</span><span class="sxs-lookup"><span data-stu-id="96230-124">Accept</span></span>|<span data-ttu-id="96230-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96230-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96230-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="96230-126">Request body</span></span>
<span data-ttu-id="96230-127">要求本文で、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="96230-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="96230-128">次の表に、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="96230-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="96230-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96230-129">Property</span></span>|<span data-ttu-id="96230-130">型</span><span class="sxs-lookup"><span data-stu-id="96230-130">Type</span></span>|<span data-ttu-id="96230-131">説明</span><span class="sxs-lookup"><span data-stu-id="96230-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96230-132">id</span><span class="sxs-lookup"><span data-stu-id="96230-132">id</span></span>|<span data-ttu-id="96230-133">文字列</span><span class="sxs-lookup"><span data-stu-id="96230-133">String</span></span>|<span data-ttu-id="96230-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="96230-134">The GUID for the object</span></span>|
|<span data-ttu-id="96230-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="96230-135">orderIdentifier</span></span>|<span data-ttu-id="96230-136">String</span><span class="sxs-lookup"><span data-stu-id="96230-136">String</span></span>|<span data-ttu-id="96230-137">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="96230-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="96230-138">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="96230-138">serialNumber</span></span>|<span data-ttu-id="96230-139">String</span><span class="sxs-lookup"><span data-stu-id="96230-139">String</span></span>|<span data-ttu-id="96230-140">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="96230-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="96230-141">productKey</span><span class="sxs-lookup"><span data-stu-id="96230-141">productKey</span></span>|<span data-ttu-id="96230-142">String</span><span class="sxs-lookup"><span data-stu-id="96230-142">String</span></span>|<span data-ttu-id="96230-143">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="96230-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="96230-144">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="96230-144">hardwareIdentifier</span></span>|<span data-ttu-id="96230-145">Binary</span><span class="sxs-lookup"><span data-stu-id="96230-145">Binary</span></span>|<span data-ttu-id="96230-146">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="96230-146">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="96230-147">state</span><span class="sxs-lookup"><span data-stu-id="96230-147">state</span></span>|[<span data-ttu-id="96230-148">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="96230-148">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="96230-149">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="96230-149">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="96230-150">応答</span><span class="sxs-lookup"><span data-stu-id="96230-150">Response</span></span>
<span data-ttu-id="96230-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="96230-151">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96230-152">例</span><span class="sxs-lookup"><span data-stu-id="96230-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="96230-153">要求</span><span class="sxs-lookup"><span data-stu-id="96230-153">Request</span></span>
<span data-ttu-id="96230-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96230-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="96230-155">応答</span><span class="sxs-lookup"><span data-stu-id="96230-155">Response</span></span>
<span data-ttu-id="96230-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="96230-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




