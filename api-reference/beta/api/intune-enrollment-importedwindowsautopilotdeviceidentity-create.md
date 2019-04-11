---
title: Create importedWindowsAutopilotDeviceIdentity
description: 新規で importedWindowsAutopilotDeviceIdentity オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7a35693408b214d028af90945e0d3179af83395
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774765"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="c2181-103">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c2181-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="c2181-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2181-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2181-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2181-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2181-106">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c2181-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2181-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c2181-107">Prerequisites</span></span>
<span data-ttu-id="c2181-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2181-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2181-110">Permission type</span></span>|<span data-ttu-id="c2181-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2181-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2181-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2181-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2181-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2181-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c2181-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2181-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2181-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2181-115">Not supported.</span></span>|
|<span data-ttu-id="c2181-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2181-116">Application</span></span>|<span data-ttu-id="c2181-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2181-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2181-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2181-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="c2181-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2181-119">Request headers</span></span>
|<span data-ttu-id="c2181-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2181-120">Header</span></span>|<span data-ttu-id="c2181-121">値</span><span class="sxs-lookup"><span data-stu-id="c2181-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2181-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2181-122">Authorization</span></span>|<span data-ttu-id="c2181-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2181-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2181-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c2181-124">Accept</span></span>|<span data-ttu-id="c2181-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2181-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2181-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2181-126">Request body</span></span>
<span data-ttu-id="c2181-127">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2181-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="c2181-128">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c2181-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="c2181-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2181-129">Property</span></span>|<span data-ttu-id="c2181-130">型</span><span class="sxs-lookup"><span data-stu-id="c2181-130">Type</span></span>|<span data-ttu-id="c2181-131">説明</span><span class="sxs-lookup"><span data-stu-id="c2181-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2181-132">id</span><span class="sxs-lookup"><span data-stu-id="c2181-132">id</span></span>|<span data-ttu-id="c2181-133">String</span><span class="sxs-lookup"><span data-stu-id="c2181-133">String</span></span>|<span data-ttu-id="c2181-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="c2181-134">The GUID for the object</span></span>|
|<span data-ttu-id="c2181-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="c2181-135">orderIdentifier</span></span>|<span data-ttu-id="c2181-136">String</span><span class="sxs-lookup"><span data-stu-id="c2181-136">String</span></span>|<span data-ttu-id="c2181-137">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="c2181-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c2181-138">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="c2181-138">serialNumber</span></span>|<span data-ttu-id="c2181-139">文字列</span><span class="sxs-lookup"><span data-stu-id="c2181-139">String</span></span>|<span data-ttu-id="c2181-140">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="c2181-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c2181-141">productKey</span><span class="sxs-lookup"><span data-stu-id="c2181-141">productKey</span></span>|<span data-ttu-id="c2181-142">String</span><span class="sxs-lookup"><span data-stu-id="c2181-142">String</span></span>|<span data-ttu-id="c2181-143">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="c2181-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c2181-144">のようにします。</span><span class="sxs-lookup"><span data-stu-id="c2181-144">importId</span></span>|<span data-ttu-id="c2181-145">文字列</span><span class="sxs-lookup"><span data-stu-id="c2181-145">String</span></span>|<span data-ttu-id="c2181-146">Windows 自動操縦デバイスのインポート Id。</span><span class="sxs-lookup"><span data-stu-id="c2181-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c2181-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="c2181-147">hardwareIdentifier</span></span>|<span data-ttu-id="c2181-148">Binary</span><span class="sxs-lookup"><span data-stu-id="c2181-148">Binary</span></span>|<span data-ttu-id="c2181-149">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="c2181-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="c2181-150">state</span><span class="sxs-lookup"><span data-stu-id="c2181-150">state</span></span>|[<span data-ttu-id="c2181-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="c2181-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="c2181-152">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="c2181-152">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="c2181-153">応答</span><span class="sxs-lookup"><span data-stu-id="c2181-153">Response</span></span>
<span data-ttu-id="c2181-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c2181-154">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2181-155">例</span><span class="sxs-lookup"><span data-stu-id="c2181-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2181-156">要求</span><span class="sxs-lookup"><span data-stu-id="c2181-156">Request</span></span>
<span data-ttu-id="c2181-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2181-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 575

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
  }
}
```

### <a name="response"></a><span data-ttu-id="c2181-158">応答</span><span class="sxs-lookup"><span data-stu-id="c2181-158">Response</span></span>
<span data-ttu-id="c2181-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c2181-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 624

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
  }
}
```





