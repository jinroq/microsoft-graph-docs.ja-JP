---
title: WindowsOfficeClientConfiguration を取得します。
description: セキュリティ以外の特定のポリシーの windowsOfficeClientConfiguration オブジェクトを取得します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a53fde0620e6240923dc4093a1a28d86a3c517e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955759"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="0808f-103">WindowsOfficeClientConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="0808f-103">Get windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="0808f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0808f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0808f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0808f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0808f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0808f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0808f-107">セキュリティ以外の特定のポリシーの[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0808f-107">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0808f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0808f-108">Prerequisites</span></span>
<span data-ttu-id="0808f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0808f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0808f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0808f-111">Permission type</span></span>|<span data-ttu-id="0808f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0808f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0808f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0808f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0808f-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0808f-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0808f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0808f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0808f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0808f-116">Not supported.</span></span>|
|<span data-ttu-id="0808f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0808f-117">Application</span></span>|<span data-ttu-id="0808f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0808f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0808f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0808f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0808f-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0808f-120">Optional query parameters</span></span>
<span data-ttu-id="0808f-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0808f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0808f-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0808f-122">Request headers</span></span>
|<span data-ttu-id="0808f-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0808f-123">Header</span></span>|<span data-ttu-id="0808f-124">値</span><span class="sxs-lookup"><span data-stu-id="0808f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0808f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0808f-125">Authorization</span></span>|<span data-ttu-id="0808f-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0808f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0808f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0808f-127">Accept</span></span>|<span data-ttu-id="0808f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0808f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0808f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0808f-129">Request body</span></span>
<span data-ttu-id="0808f-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0808f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0808f-131">応答</span><span class="sxs-lookup"><span data-stu-id="0808f-131">Response</span></span>
<span data-ttu-id="0808f-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0808f-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0808f-133">例</span><span class="sxs-lookup"><span data-stu-id="0808f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="0808f-134">要求</span><span class="sxs-lookup"><span data-stu-id="0808f-134">Request</span></span>
<span data-ttu-id="0808f-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0808f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="0808f-136">応答</span><span class="sxs-lookup"><span data-stu-id="0808f-136">Response</span></span>
<span data-ttu-id="0808f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0808f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1144

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
    "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
    "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
    "policyPayload": "<Unknown Primitive Type Edm.Stream>",
    "description": "Description value",
    "displayName": "Display Name value",
    "priority": 8,
    "userCheckinSummary": {
      "@odata.type": "microsoft.graph.officeUserCheckinSummary",
      "succeededUserCount": 2,
      "failedUserCount": 15
    },
    "checkinStatuses": [
      {
        "@odata.type": "microsoft.graph.officeClientCheckinStatus",
        "userPrincipalName": "User Principal Name value",
        "deviceName": "Device Name value",
        "devicePlatform": "Device Platform value",
        "devicePlatformVersion": "Device Platform Version value",
        "wasSuccessful": true,
        "userId": "User Id value",
        "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
        "errorMessage": "Error Message value",
        "appliedPolicies": [
          "Applied Policies value"
        ]
      }
    ]
  }
}
```



