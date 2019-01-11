---
title: Get iosManagedAppRegistration
description: iosManagedAppRegistration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bac379de3e185c2ae9f9e2627bafdab0e7c7ce45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844745"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="8062b-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8062b-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="8062b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8062b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8062b-105">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8062b-105">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8062b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8062b-106">Prerequisites</span></span>
<span data-ttu-id="8062b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8062b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8062b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8062b-109">Permission type</span></span>|<span data-ttu-id="8062b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8062b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8062b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8062b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8062b-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8062b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8062b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8062b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8062b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8062b-114">Not supported.</span></span>|
|<span data-ttu-id="8062b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8062b-115">Application</span></span>|<span data-ttu-id="8062b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8062b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8062b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8062b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8062b-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8062b-118">Optional query parameters</span></span>
<span data-ttu-id="8062b-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8062b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8062b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8062b-120">Request headers</span></span>
|<span data-ttu-id="8062b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8062b-121">Header</span></span>|<span data-ttu-id="8062b-122">値</span><span class="sxs-lookup"><span data-stu-id="8062b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8062b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8062b-123">Authorization</span></span>|<span data-ttu-id="8062b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8062b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8062b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8062b-125">Accept</span></span>|<span data-ttu-id="8062b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8062b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8062b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8062b-127">Request body</span></span>
<span data-ttu-id="8062b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8062b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8062b-129">応答</span><span class="sxs-lookup"><span data-stu-id="8062b-129">Response</span></span>
<span data-ttu-id="8062b-130">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8062b-130">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8062b-131">例</span><span class="sxs-lookup"><span data-stu-id="8062b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8062b-132">要求</span><span class="sxs-lookup"><span data-stu-id="8062b-132">Request</span></span>
<span data-ttu-id="8062b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8062b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="8062b-134">応答</span><span class="sxs-lookup"><span data-stu-id="8062b-134">Response</span></span>
<span data-ttu-id="8062b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8062b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 800

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "flaggedReasons": [
      "rootedDevice"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
      "bundleId": "Bundle Id value"
    },
    "id": "47632c19-2c19-4763-192c-6347192c6347",
    "version": "Version value"
  }
}
```



