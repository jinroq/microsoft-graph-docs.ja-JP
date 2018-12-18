---
title: OfficeClientConfiguration を取得します。
description: 特定のポリシーを取得します。
author: tfitzmac
ms.openlocfilehash: 34fcde21ae4225e224b6e2b6811ce93b19e6990f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338130"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="a3e15-103">OfficeClientConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3e15-103">Get officeClientConfiguration</span></span>

> <span data-ttu-id="a3e15-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3e15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3e15-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3e15-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3e15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3e15-107">特定のポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="a3e15-107">Get a specific policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3e15-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3e15-108">Prerequisites</span></span>
<span data-ttu-id="a3e15-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3e15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3e15-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3e15-111">Permission type</span></span>|<span data-ttu-id="a3e15-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3e15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3e15-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3e15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3e15-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3e15-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3e15-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3e15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3e15-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e15-116">Not supported.</span></span>|
|<span data-ttu-id="a3e15-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3e15-117">Application</span></span>|<span data-ttu-id="a3e15-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e15-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3e15-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3e15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3e15-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a3e15-120">Optional query parameters</span></span>
<span data-ttu-id="a3e15-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a3e15-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a3e15-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3e15-122">Request headers</span></span>
|<span data-ttu-id="a3e15-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3e15-123">Header</span></span>|<span data-ttu-id="a3e15-124">値</span><span class="sxs-lookup"><span data-stu-id="a3e15-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3e15-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3e15-125">Authorization</span></span>|<span data-ttu-id="a3e15-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a3e15-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3e15-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a3e15-127">Accept</span></span>|<span data-ttu-id="a3e15-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a3e15-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3e15-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3e15-129">Request body</span></span>
<span data-ttu-id="a3e15-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3e15-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3e15-131">応答</span><span class="sxs-lookup"><span data-stu-id="a3e15-131">Response</span></span>
<span data-ttu-id="a3e15-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a3e15-132">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3e15-133">例</span><span class="sxs-lookup"><span data-stu-id="a3e15-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3e15-134">要求</span><span class="sxs-lookup"><span data-stu-id="a3e15-134">Request</span></span>
<span data-ttu-id="a3e15-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3e15-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="a3e15-136">応答</span><span class="sxs-lookup"><span data-stu-id="a3e15-136">Response</span></span>
<span data-ttu-id="a3e15-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3e15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfiguration",
    "id": "362ce0f0-e0f0-362c-f0e0-2c36f0e02c36",
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



