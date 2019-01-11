---
title: リスト windowsOfficeClientSecurityConfigurations
description: WindowsOfficeClientSecurityConfiguration オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 407b89fc9c5c7fefba0c9eec8801fa10df9500fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813917"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="1e879-103">リスト windowsOfficeClientSecurityConfigurations</span><span class="sxs-lookup"><span data-stu-id="1e879-103">List windowsOfficeClientSecurityConfigurations</span></span>

> <span data-ttu-id="1e879-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e879-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e879-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e879-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e879-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e879-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e879-107">[WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1e879-107">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e879-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1e879-108">Prerequisites</span></span>
<span data-ttu-id="1e879-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e879-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e879-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e879-111">Permission type</span></span>|<span data-ttu-id="1e879-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e879-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e879-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e879-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e879-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e879-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1e879-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e879-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e879-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e879-116">Not supported.</span></span>|
|<span data-ttu-id="1e879-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e879-117">Application</span></span>|<span data-ttu-id="1e879-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e879-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e879-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e879-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e879-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e879-120">Request headers</span></span>
|<span data-ttu-id="1e879-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e879-121">Header</span></span>|<span data-ttu-id="1e879-122">値</span><span class="sxs-lookup"><span data-stu-id="1e879-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e879-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e879-123">Authorization</span></span>|<span data-ttu-id="1e879-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1e879-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e879-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e879-125">Accept</span></span>|<span data-ttu-id="1e879-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e879-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e879-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e879-127">Request body</span></span>
<span data-ttu-id="1e879-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e879-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e879-129">応答</span><span class="sxs-lookup"><span data-stu-id="1e879-129">Response</span></span>
<span data-ttu-id="1e879-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1e879-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e879-131">例</span><span class="sxs-lookup"><span data-stu-id="1e879-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e879-132">要求</span><span class="sxs-lookup"><span data-stu-id="1e879-132">Request</span></span>
<span data-ttu-id="1e879-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e879-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="1e879-134">応答</span><span class="sxs-lookup"><span data-stu-id="1e879-134">Response</span></span>
<span data-ttu-id="1e879-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e879-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1222

{
  "value": [
    {
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
  ]
}
```



