---
title: importedWindowsAutopilotDeviceIdentity の更新
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティを更新します。
ms.openlocfilehash: 7b5d79893ec30c203d4272d652ac43a225a37ec5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073423"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="9ed86-103">importedWindowsAutopilotDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="9ed86-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="9ed86-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ed86-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ed86-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ed86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ed86-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ed86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ed86-107">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9ed86-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ed86-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9ed86-108">Prerequisites</span></span>
<span data-ttu-id="9ed86-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ed86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed86-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ed86-111">Permission type</span></span>|<span data-ttu-id="9ed86-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ed86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ed86-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ed86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ed86-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed86-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9ed86-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ed86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ed86-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ed86-116">Not supported.</span></span>|
|<span data-ttu-id="9ed86-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ed86-117">Application</span></span>|<span data-ttu-id="9ed86-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ed86-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ed86-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ed86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="9ed86-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ed86-120">Request headers</span></span>
|<span data-ttu-id="9ed86-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ed86-121">Header</span></span>|<span data-ttu-id="9ed86-122">値</span><span class="sxs-lookup"><span data-stu-id="9ed86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ed86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed86-123">Authorization</span></span>|<span data-ttu-id="9ed86-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9ed86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ed86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ed86-125">Accept</span></span>|<span data-ttu-id="9ed86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ed86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ed86-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ed86-127">Request body</span></span>
<span data-ttu-id="9ed86-128">要求本文で、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ed86-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="9ed86-129">次の表に、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9ed86-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="9ed86-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ed86-130">Property</span></span>|<span data-ttu-id="9ed86-131">型</span><span class="sxs-lookup"><span data-stu-id="9ed86-131">Type</span></span>|<span data-ttu-id="9ed86-132">説明</span><span class="sxs-lookup"><span data-stu-id="9ed86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ed86-133">id</span><span class="sxs-lookup"><span data-stu-id="9ed86-133">id</span></span>|<span data-ttu-id="9ed86-134">String</span><span class="sxs-lookup"><span data-stu-id="9ed86-134">String</span></span>|<span data-ttu-id="9ed86-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="9ed86-135">The GUID for the object</span></span>|
|<span data-ttu-id="9ed86-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="9ed86-136">orderIdentifier</span></span>|<span data-ttu-id="9ed86-137">String</span><span class="sxs-lookup"><span data-stu-id="9ed86-137">String</span></span>|<span data-ttu-id="9ed86-138">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="9ed86-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9ed86-139">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="9ed86-139">serialNumber</span></span>|<span data-ttu-id="9ed86-140">String</span><span class="sxs-lookup"><span data-stu-id="9ed86-140">String</span></span>|<span data-ttu-id="9ed86-141">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="9ed86-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9ed86-142">productKey</span><span class="sxs-lookup"><span data-stu-id="9ed86-142">productKey</span></span>|<span data-ttu-id="9ed86-143">String</span><span class="sxs-lookup"><span data-stu-id="9ed86-143">String</span></span>|<span data-ttu-id="9ed86-144">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="9ed86-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9ed86-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="9ed86-145">hardwareIdentifier</span></span>|<span data-ttu-id="9ed86-146">バイナリ</span><span class="sxs-lookup"><span data-stu-id="9ed86-146">Binary</span></span>|<span data-ttu-id="9ed86-147">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="9ed86-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9ed86-148">状態</span><span class="sxs-lookup"><span data-stu-id="9ed86-148">state</span></span>|[<span data-ttu-id="9ed86-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="9ed86-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="9ed86-150">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="9ed86-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="9ed86-151">応答</span><span class="sxs-lookup"><span data-stu-id="9ed86-151">Response</span></span>
<span data-ttu-id="9ed86-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ed86-152">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ed86-153">例</span><span class="sxs-lookup"><span data-stu-id="9ed86-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ed86-154">要求</span><span class="sxs-lookup"><span data-stu-id="9ed86-154">Request</span></span>
<span data-ttu-id="9ed86-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ed86-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ed86-156">応答</span><span class="sxs-lookup"><span data-stu-id="9ed86-156">Response</span></span>
<span data-ttu-id="9ed86-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ed86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




