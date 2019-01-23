---
title: Create importedWindowsAutopilotDeviceIdentity
description: 新規で importedWindowsAutopilotDeviceIdentity オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c951e6b0489d5d42035d6f415efe64a8b6fb5d3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400726"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="94f31-103">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="94f31-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="94f31-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="94f31-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="94f31-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94f31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94f31-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94f31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94f31-107">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="94f31-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94f31-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="94f31-108">Prerequisites</span></span>
<span data-ttu-id="94f31-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94f31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="94f31-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94f31-111">Permission type</span></span>|<span data-ttu-id="94f31-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="94f31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94f31-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94f31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94f31-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f31-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94f31-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94f31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94f31-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94f31-116">Not supported.</span></span>|
|<span data-ttu-id="94f31-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94f31-117">Application</span></span>|<span data-ttu-id="94f31-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94f31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94f31-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94f31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="94f31-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94f31-120">Request headers</span></span>
|<span data-ttu-id="94f31-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94f31-121">Header</span></span>|<span data-ttu-id="94f31-122">値</span><span class="sxs-lookup"><span data-stu-id="94f31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94f31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94f31-123">Authorization</span></span>|<span data-ttu-id="94f31-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="94f31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94f31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="94f31-125">Accept</span></span>|<span data-ttu-id="94f31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94f31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94f31-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="94f31-127">Request body</span></span>
<span data-ttu-id="94f31-128">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="94f31-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="94f31-129">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="94f31-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="94f31-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94f31-130">Property</span></span>|<span data-ttu-id="94f31-131">型</span><span class="sxs-lookup"><span data-stu-id="94f31-131">Type</span></span>|<span data-ttu-id="94f31-132">説明</span><span class="sxs-lookup"><span data-stu-id="94f31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94f31-133">id</span><span class="sxs-lookup"><span data-stu-id="94f31-133">id</span></span>|<span data-ttu-id="94f31-134">String</span><span class="sxs-lookup"><span data-stu-id="94f31-134">String</span></span>|<span data-ttu-id="94f31-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="94f31-135">The GUID for the object</span></span>|
|<span data-ttu-id="94f31-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="94f31-136">orderIdentifier</span></span>|<span data-ttu-id="94f31-137">String</span><span class="sxs-lookup"><span data-stu-id="94f31-137">String</span></span>|<span data-ttu-id="94f31-138">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="94f31-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94f31-139">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="94f31-139">serialNumber</span></span>|<span data-ttu-id="94f31-140">String</span><span class="sxs-lookup"><span data-stu-id="94f31-140">String</span></span>|<span data-ttu-id="94f31-141">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="94f31-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94f31-142">productKey</span><span class="sxs-lookup"><span data-stu-id="94f31-142">productKey</span></span>|<span data-ttu-id="94f31-143">String</span><span class="sxs-lookup"><span data-stu-id="94f31-143">String</span></span>|<span data-ttu-id="94f31-144">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="94f31-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94f31-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="94f31-145">hardwareIdentifier</span></span>|<span data-ttu-id="94f31-146">Binary</span><span class="sxs-lookup"><span data-stu-id="94f31-146">Binary</span></span>|<span data-ttu-id="94f31-147">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="94f31-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94f31-148">state</span><span class="sxs-lookup"><span data-stu-id="94f31-148">state</span></span>|[<span data-ttu-id="94f31-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="94f31-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="94f31-150">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="94f31-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="94f31-151">応答</span><span class="sxs-lookup"><span data-stu-id="94f31-151">Response</span></span>
<span data-ttu-id="94f31-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94f31-152">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94f31-153">例</span><span class="sxs-lookup"><span data-stu-id="94f31-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="94f31-154">要求</span><span class="sxs-lookup"><span data-stu-id="94f31-154">Request</span></span>
<span data-ttu-id="94f31-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94f31-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="94f31-156">応答</span><span class="sxs-lookup"><span data-stu-id="94f31-156">Response</span></span>
<span data-ttu-id="94f31-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94f31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




