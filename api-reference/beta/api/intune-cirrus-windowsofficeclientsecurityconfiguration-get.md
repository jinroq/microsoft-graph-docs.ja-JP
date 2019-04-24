---
title: windowsOfficeClientSecurityConfiguration を取得する
description: 特定のセキュリティポリシー windowsOfficeClientSecurityConfiguration オブジェクトを取得します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 02edba061958739dd0dac43151e027b414be19d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483419"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="0ea00-103">windowsOfficeClientSecurityConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="0ea00-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="0ea00-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ea00-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ea00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ea00-106">特定のセキュリティポリシー [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ea00-106">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ea00-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0ea00-107">Prerequisites</span></span>
<span data-ttu-id="0ea00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ea00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea00-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ea00-110">Permission type</span></span>|<span data-ttu-id="0ea00-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ea00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ea00-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ea00-113">devicemanagementconfiguration をすべて取得します。</span><span class="sxs-lookup"><span data-stu-id="0ea00-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0ea00-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ea00-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea00-115">Not supported.</span></span>|
|<span data-ttu-id="0ea00-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ea00-116">Application</span></span>|<span data-ttu-id="0ea00-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ea00-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ea00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ea00-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0ea00-119">Optional query parameters</span></span>
<span data-ttu-id="0ea00-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0ea00-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ea00-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ea00-121">Request headers</span></span>
|<span data-ttu-id="0ea00-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ea00-122">Header</span></span>|<span data-ttu-id="0ea00-123">値</span><span class="sxs-lookup"><span data-stu-id="0ea00-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ea00-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea00-124">Authorization</span></span>|<span data-ttu-id="0ea00-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ea00-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ea00-126">承諾</span><span class="sxs-lookup"><span data-stu-id="0ea00-126">Accept</span></span>|<span data-ttu-id="0ea00-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0ea00-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ea00-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ea00-128">Request body</span></span>
<span data-ttu-id="0ea00-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0ea00-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea00-130">応答</span><span class="sxs-lookup"><span data-stu-id="0ea00-130">Response</span></span>
<span data-ttu-id="0ea00-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0ea00-131">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea00-132">例</span><span class="sxs-lookup"><span data-stu-id="0ea00-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ea00-133">要求</span><span class="sxs-lookup"><span data-stu-id="0ea00-133">Request</span></span>
<span data-ttu-id="0ea00-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ea00-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="0ea00-135">応答</span><span class="sxs-lookup"><span data-stu-id="0ea00-135">Response</span></span>
<span data-ttu-id="0ea00-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ea00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



