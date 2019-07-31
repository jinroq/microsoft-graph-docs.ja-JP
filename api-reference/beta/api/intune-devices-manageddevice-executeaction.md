---
title: executeAction アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5afcbdf1847f3e8b06b6f65dc1c3c6b292f6c99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985862"
---
# <a name="executeaction-action"></a><span data-ttu-id="bba1b-103">executeAction アクション</span><span class="sxs-lookup"><span data-stu-id="bba1b-103">executeAction action</span></span>

> <span data-ttu-id="bba1b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bba1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bba1b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bba1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bba1b-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bba1b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bba1b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bba1b-107">Prerequisites</span></span>
<span data-ttu-id="bba1b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bba1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bba1b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bba1b-110">Permission type</span></span>|<span data-ttu-id="bba1b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bba1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bba1b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bba1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bba1b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="bba1b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="bba1b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bba1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bba1b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bba1b-115">Not supported.</span></span>|
|<span data-ttu-id="bba1b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bba1b-116">Application</span></span>|<span data-ttu-id="bba1b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bba1b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bba1b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bba1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="bba1b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bba1b-119">Request headers</span></span>
|<span data-ttu-id="bba1b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bba1b-120">Header</span></span>|<span data-ttu-id="bba1b-121">値</span><span class="sxs-lookup"><span data-stu-id="bba1b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bba1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bba1b-122">Authorization</span></span>|<span data-ttu-id="bba1b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bba1b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bba1b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bba1b-124">Accept</span></span>|<span data-ttu-id="bba1b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bba1b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bba1b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bba1b-126">Request body</span></span>
<span data-ttu-id="bba1b-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bba1b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bba1b-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="bba1b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bba1b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bba1b-129">Property</span></span>|<span data-ttu-id="bba1b-130">型</span><span class="sxs-lookup"><span data-stu-id="bba1b-130">Type</span></span>|<span data-ttu-id="bba1b-131">説明</span><span class="sxs-lookup"><span data-stu-id="bba1b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bba1b-132">actionName</span><span class="sxs-lookup"><span data-stu-id="bba1b-132">actionName</span></span>|[<span data-ttu-id="bba1b-133">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="bba1b-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="bba1b-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bba1b-134">Not yet documented</span></span>|
|<span data-ttu-id="bba1b-135">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="bba1b-135">keepEnrollmentData</span></span>|<span data-ttu-id="bba1b-136">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bba1b-136">Boolean</span></span>|<span data-ttu-id="bba1b-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bba1b-137">Not yet documented</span></span>|
|<span data-ttu-id="bba1b-138">keepUserData</span><span class="sxs-lookup"><span data-stu-id="bba1b-138">keepUserData</span></span>|<span data-ttu-id="bba1b-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="bba1b-139">Boolean</span></span>|<span data-ttu-id="bba1b-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bba1b-140">Not yet documented</span></span>|
|<span data-ttu-id="bba1b-141">deviceIds</span><span class="sxs-lookup"><span data-stu-id="bba1b-141">deviceIds</span></span>|<span data-ttu-id="bba1b-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bba1b-142">String collection</span></span>|<span data-ttu-id="bba1b-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bba1b-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bba1b-144">応答</span><span class="sxs-lookup"><span data-stu-id="bba1b-144">Response</span></span>
<span data-ttu-id="bba1b-145">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[Bulkmanageddeviceactionresult](../resources/intune-devices-bulkmanageddeviceactionresult.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="bba1b-145">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bba1b-146">例</span><span class="sxs-lookup"><span data-stu-id="bba1b-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="bba1b-147">要求</span><span class="sxs-lookup"><span data-stu-id="bba1b-147">Request</span></span>
<span data-ttu-id="bba1b-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bba1b-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 134

{
  "actionName": "delete",
  "keepEnrollmentData": true,
  "keepUserData": true,
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="bba1b-149">応答</span><span class="sxs-lookup"><span data-stu-id="bba1b-149">Response</span></span>
<span data-ttu-id="bba1b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bba1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





