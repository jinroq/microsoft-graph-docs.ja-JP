---
title: 作業中の作業のトラブルシューティングイベントを取得する
description: このイベントオブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5d6490bf33733683dbaf4459b6bdc8ff9c2b2fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347396"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="3a911-103">作業中の作業のトラブルシューティングイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="3a911-103">Get appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="3a911-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a911-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a911-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a911-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a911-106">この[イベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3a911-106">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a911-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3a911-107">Prerequisites</span></span>
<span data-ttu-id="3a911-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a911-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a911-110">Permission type</span></span>|<span data-ttu-id="3a911-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a911-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a911-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a911-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a911-113">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="3a911-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="3a911-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a911-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a911-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a911-115">Not supported.</span></span>|
|<span data-ttu-id="3a911-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a911-116">Application</span></span>|<span data-ttu-id="3a911-117">\* \* TODO: AppOnly スコープを決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="3a911-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a911-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a911-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a911-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a911-119">Optional query parameters</span></span>
<span data-ttu-id="3a911-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3a911-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a911-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a911-121">Request headers</span></span>
|<span data-ttu-id="3a911-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a911-122">Header</span></span>|<span data-ttu-id="3a911-123">値</span><span class="sxs-lookup"><span data-stu-id="3a911-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a911-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a911-124">Authorization</span></span>|<span data-ttu-id="3a911-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a911-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a911-126">承諾</span><span class="sxs-lookup"><span data-stu-id="3a911-126">Accept</span></span>|<span data-ttu-id="3a911-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3a911-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a911-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a911-128">Request body</span></span>
<span data-ttu-id="3a911-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3a911-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a911-130">応答</span><span class="sxs-lookup"><span data-stu-id="3a911-130">Response</span></span>
<span data-ttu-id="3a911-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[りんご Evpptokenのトラブルシューティングイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3a911-131">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a911-132">例</span><span class="sxs-lookup"><span data-stu-id="3a911-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a911-133">要求</span><span class="sxs-lookup"><span data-stu-id="3a911-133">Request</span></span>
<span data-ttu-id="3a911-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a911-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="3a911-135">応答</span><span class="sxs-lookup"><span data-stu-id="3a911-135">Response</span></span>
<span data-ttu-id="3a911-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3a911-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1003

{
  "value": {
    "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
    "id": "09295f26-5f26-0929-265f-2909265f2909",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "troubleshootingErrorDetails": {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
      "context": "Context value",
      "failure": "Failure value",
      "failureDetails": "Failure Details value",
      "remediation": "Remediation value",
      "resources": [
        {
          "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
          "text": "Text value",
          "link": "Link value"
        }
      ]
    },
    "eventName": "Event Name value",
    "additionalInformation": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "tokenId": "Token Id value"
  }
}
```






