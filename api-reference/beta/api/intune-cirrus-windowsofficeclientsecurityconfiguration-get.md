---
title: WindowsOfficeClientSecurityConfiguration を取得します。
description: 特定のセキュリティ ポリシーの windowsOfficeClientSecurityConfiguration オブジェクトを取得します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a1619e7e1ed30afbc6b04f168f8e1fda2456e749
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409574"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="cf435-103">WindowsOfficeClientSecurityConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="cf435-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="cf435-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf435-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf435-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf435-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf435-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf435-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf435-107">特定のセキュリティ ポリシーの[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="cf435-107">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf435-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cf435-108">Prerequisites</span></span>
<span data-ttu-id="cf435-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf435-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf435-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf435-111">Permission type</span></span>|<span data-ttu-id="cf435-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf435-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf435-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf435-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf435-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf435-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf435-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf435-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf435-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf435-116">Not supported.</span></span>|
|<span data-ttu-id="cf435-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf435-117">Application</span></span>|<span data-ttu-id="cf435-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf435-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf435-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf435-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf435-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cf435-120">Optional query parameters</span></span>
<span data-ttu-id="cf435-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf435-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf435-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf435-122">Request headers</span></span>
|<span data-ttu-id="cf435-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf435-123">Header</span></span>|<span data-ttu-id="cf435-124">値</span><span class="sxs-lookup"><span data-stu-id="cf435-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf435-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf435-125">Authorization</span></span>|<span data-ttu-id="cf435-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cf435-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf435-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cf435-127">Accept</span></span>|<span data-ttu-id="cf435-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cf435-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf435-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf435-129">Request body</span></span>
<span data-ttu-id="cf435-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cf435-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf435-131">応答</span><span class="sxs-lookup"><span data-stu-id="cf435-131">Response</span></span>
<span data-ttu-id="cf435-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cf435-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf435-133">例</span><span class="sxs-lookup"><span data-stu-id="cf435-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf435-134">要求</span><span class="sxs-lookup"><span data-stu-id="cf435-134">Request</span></span>
<span data-ttu-id="cf435-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf435-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="cf435-136">応答</span><span class="sxs-lookup"><span data-stu-id="cf435-136">Response</span></span>
<span data-ttu-id="cf435-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf435-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
    "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
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



