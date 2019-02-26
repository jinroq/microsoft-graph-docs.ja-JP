---
title: importedWindowsAutopilotDeviceIdentity の取得
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 889f71b437ca9e08917e4e2893889a9f704d7703
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260831"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="705c0-103">importedWindowsAutopilotDeviceIdentity の取得</span><span class="sxs-lookup"><span data-stu-id="705c0-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="705c0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="705c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="705c0-105">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="705c0-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="705c0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="705c0-106">Prerequisites</span></span>
<span data-ttu-id="705c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="705c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="705c0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="705c0-109">Permission type</span></span>|<span data-ttu-id="705c0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="705c0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="705c0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="705c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="705c0-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="705c0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="705c0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="705c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="705c0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="705c0-114">Not supported.</span></span>|
|<span data-ttu-id="705c0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="705c0-115">Application</span></span>|<span data-ttu-id="705c0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="705c0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="705c0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="705c0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="705c0-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="705c0-118">Optional query parameters</span></span>
<span data-ttu-id="705c0-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="705c0-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="705c0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="705c0-120">Request headers</span></span>
|<span data-ttu-id="705c0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="705c0-121">Header</span></span>|<span data-ttu-id="705c0-122">値</span><span class="sxs-lookup"><span data-stu-id="705c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="705c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="705c0-123">Authorization</span></span>|<span data-ttu-id="705c0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="705c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="705c0-125">承諾</span><span class="sxs-lookup"><span data-stu-id="705c0-125">Accept</span></span>|<span data-ttu-id="705c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="705c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="705c0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="705c0-127">Request body</span></span>
<span data-ttu-id="705c0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="705c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="705c0-129">応答</span><span class="sxs-lookup"><span data-stu-id="705c0-129">Response</span></span>
<span data-ttu-id="705c0-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="705c0-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="705c0-131">例</span><span class="sxs-lookup"><span data-stu-id="705c0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="705c0-132">要求</span><span class="sxs-lookup"><span data-stu-id="705c0-132">Request</span></span>
<span data-ttu-id="705c0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="705c0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="705c0-134">応答</span><span class="sxs-lookup"><span data-stu-id="705c0-134">Response</span></span>
<span data-ttu-id="705c0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="705c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": {
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
}
```



