---
title: OfficeClientConfiguration を取得する
description: 特定のポリシーを取得します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41e10aeac65be2c623ff0db983c9f8e889a06c89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958964"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="e7544-103">OfficeClientConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="e7544-103">Get officeClientConfiguration</span></span>

> <span data-ttu-id="e7544-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7544-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7544-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7544-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7544-106">特定のポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="e7544-106">Get a specific policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7544-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e7544-107">Prerequisites</span></span>
<span data-ttu-id="e7544-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7544-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7544-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7544-110">Permission type</span></span>|<span data-ttu-id="e7544-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7544-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7544-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7544-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7544-113">DeviceManagementConfiguration をすべて取得します。</span><span class="sxs-lookup"><span data-stu-id="e7544-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7544-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7544-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7544-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7544-115">Not supported.</span></span>|
|<span data-ttu-id="e7544-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7544-116">Application</span></span>|<span data-ttu-id="e7544-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7544-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7544-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7544-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7544-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7544-119">Optional query parameters</span></span>
<span data-ttu-id="e7544-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e7544-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e7544-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7544-121">Request headers</span></span>
|<span data-ttu-id="e7544-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7544-122">Header</span></span>|<span data-ttu-id="e7544-123">値</span><span class="sxs-lookup"><span data-stu-id="e7544-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7544-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7544-124">Authorization</span></span>|<span data-ttu-id="e7544-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7544-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7544-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e7544-126">Accept</span></span>|<span data-ttu-id="e7544-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e7544-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7544-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7544-128">Request body</span></span>
<span data-ttu-id="e7544-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7544-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7544-130">応答</span><span class="sxs-lookup"><span data-stu-id="e7544-130">Response</span></span>
<span data-ttu-id="e7544-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7544-131">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7544-132">例</span><span class="sxs-lookup"><span data-stu-id="e7544-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7544-133">要求</span><span class="sxs-lookup"><span data-stu-id="e7544-133">Request</span></span>
<span data-ttu-id="e7544-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7544-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="e7544-135">応答</span><span class="sxs-lookup"><span data-stu-id="e7544-135">Response</span></span>
<span data-ttu-id="e7544-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7544-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



