---
title: リストりんご Evpptokenトラブルシューティングイベント
description: "\"りんご Evpptokenトラブルシューティング\" イベントオブジェクトのプロパティとリレーションシップをリストします。"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d035fcd8b71298b926d133118b37ea4e05675165
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979450"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="8b95a-103">リストりんご Evpptokenトラブルシューティングイベント</span><span class="sxs-lookup"><span data-stu-id="8b95a-103">List appleVppTokenTroubleshootingEvents</span></span>

> <span data-ttu-id="8b95a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b95a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b95a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b95a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b95a-106">"[りんご Evpptokenトラブルシューティング" イベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8b95a-106">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b95a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8b95a-107">Prerequisites</span></span>
<span data-ttu-id="8b95a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b95a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b95a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b95a-110">Permission type</span></span>|<span data-ttu-id="8b95a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b95a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b95a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b95a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b95a-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b95a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8b95a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b95a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b95a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b95a-115">Not supported.</span></span>|
|<span data-ttu-id="8b95a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b95a-116">Application</span></span>|<span data-ttu-id="8b95a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b95a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b95a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b95a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8b95a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b95a-119">Request headers</span></span>
|<span data-ttu-id="8b95a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b95a-120">Header</span></span>|<span data-ttu-id="8b95a-121">値</span><span class="sxs-lookup"><span data-stu-id="8b95a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b95a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b95a-122">Authorization</span></span>|<span data-ttu-id="8b95a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b95a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b95a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8b95a-124">Accept</span></span>|<span data-ttu-id="8b95a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b95a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b95a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b95a-126">Request body</span></span>
<span data-ttu-id="8b95a-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8b95a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b95a-128">応答</span><span class="sxs-lookup"><span data-stu-id="8b95a-128">Response</span></span>
<span data-ttu-id="8b95a-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、[りんご Evpptokenのトラブルシューティングイベント](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8b95a-129">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b95a-130">例</span><span class="sxs-lookup"><span data-stu-id="8b95a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b95a-131">要求</span><span class="sxs-lookup"><span data-stu-id="8b95a-131">Request</span></span>
<span data-ttu-id="8b95a-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b95a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="8b95a-133">応答</span><span class="sxs-lookup"><span data-stu-id="8b95a-133">Response</span></span>
<span data-ttu-id="8b95a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8b95a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1071

{
  "value": [
    {
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
  ]
}
```





