---
title: importedWindowsAutopilotDeviceIdentity の更新
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9631e2c44e89adc14e37872f8e837ce756777e74
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980955"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="1f3f6-103">importedWindowsAutopilotDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="1f3f6-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="1f3f6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f3f6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f3f6-106">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f3f6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1f3f6-107">Prerequisites</span></span>
<span data-ttu-id="1f3f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f3f6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f3f6-110">Permission type</span></span>|<span data-ttu-id="1f3f6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f3f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f3f6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f3f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f3f6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f3f6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f3f6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f3f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f3f6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-115">Not supported.</span></span>|
|<span data-ttu-id="1f3f6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f3f6-116">Application</span></span>|<span data-ttu-id="1f3f6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f3f6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f3f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="1f3f6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f3f6-119">Request headers</span></span>
|<span data-ttu-id="1f3f6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f3f6-120">Header</span></span>|<span data-ttu-id="1f3f6-121">値</span><span class="sxs-lookup"><span data-stu-id="1f3f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f3f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f3f6-122">Authorization</span></span>|<span data-ttu-id="1f3f6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f3f6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1f3f6-124">Accept</span></span>|<span data-ttu-id="1f3f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f3f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f3f6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f3f6-126">Request body</span></span>
<span data-ttu-id="1f3f6-127">要求本文で、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="1f3f6-128">次の表に、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="1f3f6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f3f6-129">Property</span></span>|<span data-ttu-id="1f3f6-130">型</span><span class="sxs-lookup"><span data-stu-id="1f3f6-130">Type</span></span>|<span data-ttu-id="1f3f6-131">説明</span><span class="sxs-lookup"><span data-stu-id="1f3f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f3f6-132">id</span><span class="sxs-lookup"><span data-stu-id="1f3f6-132">id</span></span>|<span data-ttu-id="1f3f6-133">String</span><span class="sxs-lookup"><span data-stu-id="1f3f6-133">String</span></span>|<span data-ttu-id="1f3f6-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="1f3f6-134">The GUID for the object</span></span>|
|<span data-ttu-id="1f3f6-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f3f6-135">orderIdentifier</span></span>|<span data-ttu-id="1f3f6-136">String</span><span class="sxs-lookup"><span data-stu-id="1f3f6-136">String</span></span>|<span data-ttu-id="1f3f6-137">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-137">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="1f3f6-138">-廃止</span><span class="sxs-lookup"><span data-stu-id="1f3f6-138">- Deprecate</span></span>|
|<span data-ttu-id="1f3f6-139">groupTag</span><span class="sxs-lookup"><span data-stu-id="1f3f6-139">groupTag</span></span>|<span data-ttu-id="1f3f6-140">String</span><span class="sxs-lookup"><span data-stu-id="1f3f6-140">String</span></span>|<span data-ttu-id="1f3f6-141">Windows 自動操縦デバイスのグループタグ。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-141">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f3f6-142">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="1f3f6-142">serialNumber</span></span>|<span data-ttu-id="1f3f6-143">String</span><span class="sxs-lookup"><span data-stu-id="1f3f6-143">String</span></span>|<span data-ttu-id="1f3f6-144">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-144">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f3f6-145">productKey</span><span class="sxs-lookup"><span data-stu-id="1f3f6-145">productKey</span></span>|<span data-ttu-id="1f3f6-146">String</span><span class="sxs-lookup"><span data-stu-id="1f3f6-146">String</span></span>|<span data-ttu-id="1f3f6-147">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-147">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f3f6-148">のようにします。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-148">importId</span></span>|<span data-ttu-id="1f3f6-149">String</span><span class="sxs-lookup"><span data-stu-id="1f3f6-149">String</span></span>|<span data-ttu-id="1f3f6-150">Windows 自動操縦デバイスのインポート Id。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-150">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f3f6-151">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f3f6-151">hardwareIdentifier</span></span>|<span data-ttu-id="1f3f6-152">Binary</span><span class="sxs-lookup"><span data-stu-id="1f3f6-152">Binary</span></span>|<span data-ttu-id="1f3f6-153">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-153">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1f3f6-154">state</span><span class="sxs-lookup"><span data-stu-id="1f3f6-154">state</span></span>|[<span data-ttu-id="1f3f6-155">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="1f3f6-155">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="1f3f6-156">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-156">Current state of the imported device.</span></span>|
|<span data-ttu-id="1f3f6-157">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1f3f6-157">assignedUserPrincipalName</span></span>|<span data-ttu-id="1f3f6-158">String</span><span class="sxs-lookup"><span data-stu-id="1f3f6-158">String</span></span>|<span data-ttu-id="1f3f6-159">デバイスが割り当てられるユーザーの UPN</span><span class="sxs-lookup"><span data-stu-id="1f3f6-159">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="1f3f6-160">応答</span><span class="sxs-lookup"><span data-stu-id="1f3f6-160">Response</span></span>
<span data-ttu-id="1f3f6-161">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-161">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f3f6-162">例</span><span class="sxs-lookup"><span data-stu-id="1f3f6-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f3f6-163">要求</span><span class="sxs-lookup"><span data-stu-id="1f3f6-163">Request</span></span>
<span data-ttu-id="1f3f6-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 679

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
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
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="1f3f6-165">応答</span><span class="sxs-lookup"><span data-stu-id="1f3f6-165">Response</span></span>
<span data-ttu-id="1f3f6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1f3f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 728

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
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
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```





