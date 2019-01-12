---
title: Get managedAppRegistration
description: managedAppRegistration オブジェクトのプロパティとリレーションを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cade648ed41badea25a33d4b8103590ede4dea7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920437"
---
# <a name="get-managedappregistration"></a><span data-ttu-id="ad678-103">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ad678-103">Get managedAppRegistration</span></span>

> <span data-ttu-id="ad678-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad678-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad678-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad678-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad678-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad678-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad678-107">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ad678-107">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad678-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad678-108">Prerequisites</span></span>
<span data-ttu-id="ad678-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad678-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad678-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad678-111">Permission type</span></span>|<span data-ttu-id="ad678-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad678-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad678-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad678-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad678-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad678-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ad678-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad678-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad678-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad678-116">Not supported.</span></span>|
|<span data-ttu-id="ad678-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad678-117">Application</span></span>|<span data-ttu-id="ad678-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad678-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad678-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad678-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad678-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad678-120">Optional query parameters</span></span>
<span data-ttu-id="ad678-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ad678-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ad678-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad678-122">Request headers</span></span>
|<span data-ttu-id="ad678-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad678-123">Header</span></span>|<span data-ttu-id="ad678-124">値</span><span class="sxs-lookup"><span data-stu-id="ad678-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad678-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad678-125">Authorization</span></span>|<span data-ttu-id="ad678-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ad678-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad678-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ad678-127">Accept</span></span>|<span data-ttu-id="ad678-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ad678-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad678-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad678-129">Request body</span></span>
<span data-ttu-id="ad678-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad678-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad678-131">応答</span><span class="sxs-lookup"><span data-stu-id="ad678-131">Response</span></span>
<span data-ttu-id="ad678-132">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad678-132">If successful, this method returns a `200 OK` response code and [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad678-133">例</span><span class="sxs-lookup"><span data-stu-id="ad678-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad678-134">要求</span><span class="sxs-lookup"><span data-stu-id="ad678-134">Request</span></span>
<span data-ttu-id="ad678-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad678-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="ad678-136">応答</span><span class="sxs-lookup"><span data-stu-id="ad678-136">Response</span></span>
<span data-ttu-id="ad678-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad678-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 956

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppRegistration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "managedDeviceId": "Managed Device Id value",
    "azureADDeviceId": "Azure ADDevice Id value",
    "deviceModel": "Device Model value",
    "deviceManufacturer": "Device Manufacturer value",
    "flaggedReasons": [
      "rootedDevice"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "5496aa60-aa60-5496-60aa-965460aa9654",
    "version": "Version value"
  }
}
```





