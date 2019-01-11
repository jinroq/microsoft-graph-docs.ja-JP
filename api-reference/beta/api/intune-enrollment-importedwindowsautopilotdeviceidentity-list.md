---
title: List importedWindowsAutopilotDeviceIdentities
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティとリレーションシップのリストを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d4d3148e8882aac0db0a25fb000955aaac5f6557
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838340"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="622ba-103">List importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="622ba-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="622ba-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="622ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="622ba-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="622ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="622ba-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="622ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="622ba-107">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)オブジェクトのプロパティとリレーションシップのリストを作成します。</span><span class="sxs-lookup"><span data-stu-id="622ba-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="622ba-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="622ba-108">Prerequisites</span></span>
<span data-ttu-id="622ba-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="622ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="622ba-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="622ba-111">Permission type</span></span>|<span data-ttu-id="622ba-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="622ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="622ba-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="622ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="622ba-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="622ba-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="622ba-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="622ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="622ba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="622ba-116">Not supported.</span></span>|
|<span data-ttu-id="622ba-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="622ba-117">Application</span></span>|<span data-ttu-id="622ba-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="622ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="622ba-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="622ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="622ba-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="622ba-120">Request headers</span></span>
|<span data-ttu-id="622ba-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="622ba-121">Header</span></span>|<span data-ttu-id="622ba-122">値</span><span class="sxs-lookup"><span data-stu-id="622ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="622ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="622ba-123">Authorization</span></span>|<span data-ttu-id="622ba-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="622ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="622ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="622ba-125">Accept</span></span>|<span data-ttu-id="622ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="622ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="622ba-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="622ba-127">Request body</span></span>
<span data-ttu-id="622ba-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="622ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="622ba-129">応答</span><span class="sxs-lookup"><span data-stu-id="622ba-129">Response</span></span>
<span data-ttu-id="622ba-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="622ba-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="622ba-131">例</span><span class="sxs-lookup"><span data-stu-id="622ba-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="622ba-132">要求</span><span class="sxs-lookup"><span data-stu-id="622ba-132">Request</span></span>
<span data-ttu-id="622ba-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="622ba-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="622ba-134">応答</span><span class="sxs-lookup"><span data-stu-id="622ba-134">Response</span></span>
<span data-ttu-id="622ba-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="622ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





