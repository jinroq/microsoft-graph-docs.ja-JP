---
title: Create importedWindowsAutopilotDeviceIdentity
description: 新規で importedWindowsAutopilotDeviceIdentity オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 486e9760fcefb2f92be08c3939c77f3e561b9acb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877834"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="be4ce-103">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="be4ce-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="be4ce-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="be4ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be4ce-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be4ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be4ce-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="be4ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be4ce-107">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="be4ce-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be4ce-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="be4ce-108">Prerequisites</span></span>
<span data-ttu-id="be4ce-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be4ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be4ce-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be4ce-111">Permission type</span></span>|<span data-ttu-id="be4ce-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="be4ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be4ce-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be4ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be4ce-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4ce-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="be4ce-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be4ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be4ce-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be4ce-116">Not supported.</span></span>|
|<span data-ttu-id="be4ce-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be4ce-117">Application</span></span>|<span data-ttu-id="be4ce-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be4ce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be4ce-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be4ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="be4ce-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be4ce-120">Request headers</span></span>
|<span data-ttu-id="be4ce-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be4ce-121">Header</span></span>|<span data-ttu-id="be4ce-122">値</span><span class="sxs-lookup"><span data-stu-id="be4ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be4ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be4ce-123">Authorization</span></span>|<span data-ttu-id="be4ce-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="be4ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be4ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be4ce-125">Accept</span></span>|<span data-ttu-id="be4ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be4ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be4ce-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="be4ce-127">Request body</span></span>
<span data-ttu-id="be4ce-128">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="be4ce-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="be4ce-129">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="be4ce-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="be4ce-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be4ce-130">Property</span></span>|<span data-ttu-id="be4ce-131">種類</span><span class="sxs-lookup"><span data-stu-id="be4ce-131">Type</span></span>|<span data-ttu-id="be4ce-132">説明</span><span class="sxs-lookup"><span data-stu-id="be4ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be4ce-133">ID</span><span class="sxs-lookup"><span data-stu-id="be4ce-133">id</span></span>|<span data-ttu-id="be4ce-134">String</span><span class="sxs-lookup"><span data-stu-id="be4ce-134">String</span></span>|<span data-ttu-id="be4ce-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="be4ce-135">The GUID for the object</span></span>|
|<span data-ttu-id="be4ce-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="be4ce-136">orderIdentifier</span></span>|<span data-ttu-id="be4ce-137">String</span><span class="sxs-lookup"><span data-stu-id="be4ce-137">String</span></span>|<span data-ttu-id="be4ce-138">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="be4ce-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be4ce-139">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="be4ce-139">serialNumber</span></span>|<span data-ttu-id="be4ce-140">String</span><span class="sxs-lookup"><span data-stu-id="be4ce-140">String</span></span>|<span data-ttu-id="be4ce-141">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="be4ce-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be4ce-142">productKey</span><span class="sxs-lookup"><span data-stu-id="be4ce-142">productKey</span></span>|<span data-ttu-id="be4ce-143">String</span><span class="sxs-lookup"><span data-stu-id="be4ce-143">String</span></span>|<span data-ttu-id="be4ce-144">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="be4ce-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be4ce-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="be4ce-145">hardwareIdentifier</span></span>|<span data-ttu-id="be4ce-146">Binary</span><span class="sxs-lookup"><span data-stu-id="be4ce-146">Binary</span></span>|<span data-ttu-id="be4ce-147">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="be4ce-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be4ce-148">state</span><span class="sxs-lookup"><span data-stu-id="be4ce-148">state</span></span>|[<span data-ttu-id="be4ce-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="be4ce-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="be4ce-150">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="be4ce-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="be4ce-151">応答</span><span class="sxs-lookup"><span data-stu-id="be4ce-151">Response</span></span>
<span data-ttu-id="be4ce-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be4ce-152">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be4ce-153">例</span><span class="sxs-lookup"><span data-stu-id="be4ce-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="be4ce-154">要求</span><span class="sxs-lookup"><span data-stu-id="be4ce-154">Request</span></span>
<span data-ttu-id="be4ce-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be4ce-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be4ce-156">応答</span><span class="sxs-lookup"><span data-stu-id="be4ce-156">Response</span></span>
<span data-ttu-id="be4ce-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be4ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





