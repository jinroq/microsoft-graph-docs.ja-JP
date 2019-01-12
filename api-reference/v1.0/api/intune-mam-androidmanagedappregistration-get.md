---
title: Get androidManagedAppRegistration
description: androidManagedAppRegistration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b41b4e0b5975be857f81b2282928aee3ca60336
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959021"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="4954c-103">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="4954c-103">Get androidManagedAppRegistration</span></span>

> <span data-ttu-id="4954c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4954c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4954c-105">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4954c-105">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4954c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4954c-106">Prerequisites</span></span>
<span data-ttu-id="4954c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4954c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4954c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4954c-109">Permission type</span></span>|<span data-ttu-id="4954c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4954c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4954c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4954c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4954c-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4954c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4954c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4954c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4954c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4954c-114">Not supported.</span></span>|
|<span data-ttu-id="4954c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4954c-115">Application</span></span>|<span data-ttu-id="4954c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4954c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4954c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4954c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4954c-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4954c-118">Optional query parameters</span></span>
<span data-ttu-id="4954c-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4954c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4954c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4954c-120">Request headers</span></span>
|<span data-ttu-id="4954c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4954c-121">Header</span></span>|<span data-ttu-id="4954c-122">値</span><span class="sxs-lookup"><span data-stu-id="4954c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4954c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4954c-123">Authorization</span></span>|<span data-ttu-id="4954c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4954c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4954c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4954c-125">Accept</span></span>|<span data-ttu-id="4954c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4954c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4954c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4954c-127">Request body</span></span>
<span data-ttu-id="4954c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4954c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4954c-129">応答</span><span class="sxs-lookup"><span data-stu-id="4954c-129">Response</span></span>
<span data-ttu-id="4954c-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4954c-130">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4954c-131">例</span><span class="sxs-lookup"><span data-stu-id="4954c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4954c-132">要求</span><span class="sxs-lookup"><span data-stu-id="4954c-132">Request</span></span>
<span data-ttu-id="4954c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4954c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="4954c-134">応答</span><span class="sxs-lookup"><span data-stu-id="4954c-134">Response</span></span>
<span data-ttu-id="4954c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4954c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
      "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
      "packageId": "Package Id value"
    },
    "id": "0e064997-4997-0e06-9749-060e9749060e",
    "version": "Version value"
  }
}
```



