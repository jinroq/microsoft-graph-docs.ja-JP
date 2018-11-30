---
title: List importedWindowsAutopilotDeviceIdentities
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティとリレーションシップのリストを作成します。
ms.openlocfilehash: 74387db4dbfb4055a558f1213a2670e7ed3449a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020377"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="3fa3e-103">List importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3fa3e-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="3fa3e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fa3e-105">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)オブジェクトのプロパティとリレーションシップのリストを作成します。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fa3e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3fa3e-106">Prerequisites</span></span>
<span data-ttu-id="3fa3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fa3e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3fa3e-109">Permission type</span></span>|<span data-ttu-id="3fa3e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3fa3e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fa3e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3fa3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3fa3e-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fa3e-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3fa3e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3fa3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fa3e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-114">Not supported.</span></span>|
|<span data-ttu-id="3fa3e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3fa3e-115">Application</span></span>|<span data-ttu-id="3fa3e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fa3e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3fa3e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="3fa3e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fa3e-118">Request headers</span></span>
|<span data-ttu-id="3fa3e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fa3e-119">Header</span></span>|<span data-ttu-id="3fa3e-120">値</span><span class="sxs-lookup"><span data-stu-id="3fa3e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fa3e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fa3e-121">Authorization</span></span>|<span data-ttu-id="3fa3e-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fa3e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3fa3e-123">Accept</span></span>|<span data-ttu-id="3fa3e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3fa3e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fa3e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3fa3e-125">Request body</span></span>
<span data-ttu-id="3fa3e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fa3e-127">応答</span><span class="sxs-lookup"><span data-stu-id="3fa3e-127">Response</span></span>
<span data-ttu-id="3fa3e-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa3e-129">例</span><span class="sxs-lookup"><span data-stu-id="3fa3e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fa3e-130">要求</span><span class="sxs-lookup"><span data-stu-id="3fa3e-130">Request</span></span>
<span data-ttu-id="3fa3e-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="3fa3e-132">応答</span><span class="sxs-lookup"><span data-stu-id="3fa3e-132">Response</span></span>
<span data-ttu-id="3fa3e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3fa3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
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
  ]
}
```



