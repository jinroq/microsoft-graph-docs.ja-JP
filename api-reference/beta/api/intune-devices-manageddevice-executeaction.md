---
title: executeAction アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6fc154f7b0f8b6fafded763c8fbc1276284e53f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348782"
---
# <a name="executeaction-action"></a><span data-ttu-id="3c4af-103">executeAction アクション</span><span class="sxs-lookup"><span data-stu-id="3c4af-103">executeAction action</span></span>

> <span data-ttu-id="3c4af-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c4af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c4af-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c4af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c4af-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c4af-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c4af-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3c4af-107">Prerequisites</span></span>
<span data-ttu-id="3c4af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c4af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c4af-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c4af-110">Permission type</span></span>|<span data-ttu-id="3c4af-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c4af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c4af-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c4af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c4af-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3c4af-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="3c4af-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c4af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c4af-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c4af-115">Not supported.</span></span>|
|<span data-ttu-id="3c4af-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c4af-116">Application</span></span>|<span data-ttu-id="3c4af-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3c4af-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c4af-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c4af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="3c4af-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c4af-119">Request headers</span></span>
|<span data-ttu-id="3c4af-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c4af-120">Header</span></span>|<span data-ttu-id="3c4af-121">値</span><span class="sxs-lookup"><span data-stu-id="3c4af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c4af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c4af-122">Authorization</span></span>|<span data-ttu-id="3c4af-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3c4af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c4af-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3c4af-124">Accept</span></span>|<span data-ttu-id="3c4af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c4af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c4af-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c4af-126">Request body</span></span>
<span data-ttu-id="3c4af-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c4af-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3c4af-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3c4af-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3c4af-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c4af-129">Property</span></span>|<span data-ttu-id="3c4af-130">型</span><span class="sxs-lookup"><span data-stu-id="3c4af-130">Type</span></span>|<span data-ttu-id="3c4af-131">説明</span><span class="sxs-lookup"><span data-stu-id="3c4af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c4af-132">actionName</span><span class="sxs-lookup"><span data-stu-id="3c4af-132">actionName</span></span>|[<span data-ttu-id="3c4af-133">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="3c4af-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="3c4af-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c4af-134">Not yet documented</span></span>|
|<span data-ttu-id="3c4af-135">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="3c4af-135">keepEnrollmentData</span></span>|<span data-ttu-id="3c4af-136">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="3c4af-136">Boolean</span></span>|<span data-ttu-id="3c4af-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c4af-137">Not yet documented</span></span>|
|<span data-ttu-id="3c4af-138">keepUserData</span><span class="sxs-lookup"><span data-stu-id="3c4af-138">keepUserData</span></span>|<span data-ttu-id="3c4af-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="3c4af-139">Boolean</span></span>|<span data-ttu-id="3c4af-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c4af-140">Not yet documented</span></span>|
|<span data-ttu-id="3c4af-141">deviceIds</span><span class="sxs-lookup"><span data-stu-id="3c4af-141">deviceIds</span></span>|<span data-ttu-id="3c4af-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3c4af-142">String collection</span></span>|<span data-ttu-id="3c4af-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c4af-143">Not yet documented</span></span>|
|<span data-ttu-id="3c4af-144">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="3c4af-144">notificationTitle</span></span>|<span data-ttu-id="3c4af-145">String</span><span class="sxs-lookup"><span data-stu-id="3c4af-145">String</span></span>|<span data-ttu-id="3c4af-146">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c4af-146">Not yet documented</span></span>|
|<span data-ttu-id="3c4af-147">notificationBody</span><span class="sxs-lookup"><span data-stu-id="3c4af-147">notificationBody</span></span>|<span data-ttu-id="3c4af-148">String</span><span class="sxs-lookup"><span data-stu-id="3c4af-148">String</span></span>|<span data-ttu-id="3c4af-149">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c4af-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3c4af-150">応答</span><span class="sxs-lookup"><span data-stu-id="3c4af-150">Response</span></span>
<span data-ttu-id="3c4af-151">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[Bulkmanageddeviceactionresult](../resources/intune-devices-bulkmanageddeviceactionresult.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="3c4af-151">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c4af-152">例</span><span class="sxs-lookup"><span data-stu-id="3c4af-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c4af-153">要求</span><span class="sxs-lookup"><span data-stu-id="3c4af-153">Request</span></span>
<span data-ttu-id="3c4af-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c4af-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 236

{
  "actionName": "delete",
  "keepEnrollmentData": true,
  "keepUserData": true,
  "deviceIds": [
    "Device Ids value"
  ],
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="3c4af-155">応答</span><span class="sxs-lookup"><span data-stu-id="3c4af-155">Response</span></span>
<span data-ttu-id="3c4af-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c4af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```






