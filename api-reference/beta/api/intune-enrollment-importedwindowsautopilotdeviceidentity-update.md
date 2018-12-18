---
title: importedWindowsAutopilotDeviceIdentity の更新
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 885101518f5d88261a0a0e11cfc509c470b8bf5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340510"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="cce93-103">importedWindowsAutopilotDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="cce93-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="cce93-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cce93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cce93-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cce93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cce93-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cce93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cce93-107">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cce93-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cce93-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cce93-108">Prerequisites</span></span>
<span data-ttu-id="cce93-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cce93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cce93-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cce93-111">Permission type</span></span>|<span data-ttu-id="cce93-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cce93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cce93-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cce93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cce93-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cce93-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cce93-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cce93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cce93-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cce93-116">Not supported.</span></span>|
|<span data-ttu-id="cce93-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cce93-117">Application</span></span>|<span data-ttu-id="cce93-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cce93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cce93-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cce93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="cce93-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cce93-120">Request headers</span></span>
|<span data-ttu-id="cce93-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cce93-121">Header</span></span>|<span data-ttu-id="cce93-122">値</span><span class="sxs-lookup"><span data-stu-id="cce93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cce93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cce93-123">Authorization</span></span>|<span data-ttu-id="cce93-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cce93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cce93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cce93-125">Accept</span></span>|<span data-ttu-id="cce93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cce93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cce93-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cce93-127">Request body</span></span>
<span data-ttu-id="cce93-128">要求本文で、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cce93-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="cce93-129">次の表に、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cce93-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="cce93-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cce93-130">Property</span></span>|<span data-ttu-id="cce93-131">種類</span><span class="sxs-lookup"><span data-stu-id="cce93-131">Type</span></span>|<span data-ttu-id="cce93-132">説明</span><span class="sxs-lookup"><span data-stu-id="cce93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cce93-133">ID</span><span class="sxs-lookup"><span data-stu-id="cce93-133">id</span></span>|<span data-ttu-id="cce93-134">String</span><span class="sxs-lookup"><span data-stu-id="cce93-134">String</span></span>|<span data-ttu-id="cce93-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="cce93-135">The GUID for the object</span></span>|
|<span data-ttu-id="cce93-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="cce93-136">orderIdentifier</span></span>|<span data-ttu-id="cce93-137">String</span><span class="sxs-lookup"><span data-stu-id="cce93-137">String</span></span>|<span data-ttu-id="cce93-138">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="cce93-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="cce93-139">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="cce93-139">serialNumber</span></span>|<span data-ttu-id="cce93-140">String</span><span class="sxs-lookup"><span data-stu-id="cce93-140">String</span></span>|<span data-ttu-id="cce93-141">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="cce93-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="cce93-142">productKey</span><span class="sxs-lookup"><span data-stu-id="cce93-142">productKey</span></span>|<span data-ttu-id="cce93-143">String</span><span class="sxs-lookup"><span data-stu-id="cce93-143">String</span></span>|<span data-ttu-id="cce93-144">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="cce93-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="cce93-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="cce93-145">hardwareIdentifier</span></span>|<span data-ttu-id="cce93-146">Binary</span><span class="sxs-lookup"><span data-stu-id="cce93-146">Binary</span></span>|<span data-ttu-id="cce93-147">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="cce93-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="cce93-148">state</span><span class="sxs-lookup"><span data-stu-id="cce93-148">state</span></span>|[<span data-ttu-id="cce93-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="cce93-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="cce93-150">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="cce93-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="cce93-151">応答</span><span class="sxs-lookup"><span data-stu-id="cce93-151">Response</span></span>
<span data-ttu-id="cce93-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cce93-152">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cce93-153">例</span><span class="sxs-lookup"><span data-stu-id="cce93-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="cce93-154">要求</span><span class="sxs-lookup"><span data-stu-id="cce93-154">Request</span></span>
<span data-ttu-id="cce93-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cce93-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 464

{
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

### <a name="response"></a><span data-ttu-id="cce93-156">応答</span><span class="sxs-lookup"><span data-stu-id="cce93-156">Response</span></span>
<span data-ttu-id="cce93-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cce93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





