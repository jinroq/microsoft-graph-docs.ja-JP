---
title: Create importedWindowsAutopilotDeviceIdentity
description: 新規で importedWindowsAutopilotDeviceIdentity オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c13f46d168bbb20d8166d063d3f12695ce02f50a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146257"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="f3cfc-103">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f3cfc-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="f3cfc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3cfc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3cfc-106">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3cfc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3cfc-107">Prerequisites</span></span>
<span data-ttu-id="f3cfc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f3cfc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3cfc-110">Permission type</span></span>|<span data-ttu-id="f3cfc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3cfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3cfc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3cfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3cfc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3cfc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f3cfc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3cfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3cfc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-115">Not supported.</span></span>|
|<span data-ttu-id="f3cfc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3cfc-116">Application</span></span>|<span data-ttu-id="f3cfc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3cfc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3cfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="f3cfc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3cfc-119">Request headers</span></span>
|<span data-ttu-id="f3cfc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3cfc-120">Header</span></span>|<span data-ttu-id="f3cfc-121">値</span><span class="sxs-lookup"><span data-stu-id="f3cfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3cfc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3cfc-122">Authorization</span></span>|<span data-ttu-id="f3cfc-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3cfc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f3cfc-124">Accept</span></span>|<span data-ttu-id="f3cfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3cfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3cfc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3cfc-126">Request body</span></span>
<span data-ttu-id="f3cfc-127">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="f3cfc-128">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="f3cfc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3cfc-129">Property</span></span>|<span data-ttu-id="f3cfc-130">型</span><span class="sxs-lookup"><span data-stu-id="f3cfc-130">Type</span></span>|<span data-ttu-id="f3cfc-131">説明</span><span class="sxs-lookup"><span data-stu-id="f3cfc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3cfc-132">id</span><span class="sxs-lookup"><span data-stu-id="f3cfc-132">id</span></span>|<span data-ttu-id="f3cfc-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f3cfc-133">String</span></span>|<span data-ttu-id="f3cfc-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="f3cfc-134">The GUID for the object</span></span>|
|<span data-ttu-id="f3cfc-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3cfc-135">orderIdentifier</span></span>|<span data-ttu-id="f3cfc-136">String</span><span class="sxs-lookup"><span data-stu-id="f3cfc-136">String</span></span>|<span data-ttu-id="f3cfc-137">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f3cfc-138">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="f3cfc-138">serialNumber</span></span>|<span data-ttu-id="f3cfc-139">String</span><span class="sxs-lookup"><span data-stu-id="f3cfc-139">String</span></span>|<span data-ttu-id="f3cfc-140">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f3cfc-141">productKey</span><span class="sxs-lookup"><span data-stu-id="f3cfc-141">productKey</span></span>|<span data-ttu-id="f3cfc-142">String</span><span class="sxs-lookup"><span data-stu-id="f3cfc-142">String</span></span>|<span data-ttu-id="f3cfc-143">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f3cfc-144">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3cfc-144">hardwareIdentifier</span></span>|<span data-ttu-id="f3cfc-145">Binary</span><span class="sxs-lookup"><span data-stu-id="f3cfc-145">Binary</span></span>|<span data-ttu-id="f3cfc-146">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-146">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f3cfc-147">state</span><span class="sxs-lookup"><span data-stu-id="f3cfc-147">state</span></span>|[<span data-ttu-id="f3cfc-148">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="f3cfc-148">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="f3cfc-149">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-149">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="f3cfc-150">応答</span><span class="sxs-lookup"><span data-stu-id="f3cfc-150">Response</span></span>
<span data-ttu-id="f3cfc-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-151">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3cfc-152">例</span><span class="sxs-lookup"><span data-stu-id="f3cfc-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3cfc-153">要求</span><span class="sxs-lookup"><span data-stu-id="f3cfc-153">Request</span></span>
<span data-ttu-id="f3cfc-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="f3cfc-155">応答</span><span class="sxs-lookup"><span data-stu-id="f3cfc-155">Response</span></span>
<span data-ttu-id="f3cfc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3cfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




