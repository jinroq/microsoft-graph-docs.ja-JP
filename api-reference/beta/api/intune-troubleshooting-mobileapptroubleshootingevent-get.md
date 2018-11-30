---
title: MobileAppTroubleshootingEvent を取得します。
description: MobileAppTroubleshootingEvent オブジェクトのプロパティと関係を参照してください。
ms.openlocfilehash: f70bdfb30317d1fe1033516b64efe8e046212dd7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070742"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="ca039-103">MobileAppTroubleshootingEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="ca039-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="ca039-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ca039-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca039-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca039-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca039-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca039-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca039-107">[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca039-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca039-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ca039-108">Prerequisites</span></span>
<span data-ttu-id="ca039-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca039-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca039-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca039-111">Permission type</span></span>|<span data-ttu-id="ca039-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca039-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca039-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca039-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca039-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca039-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ca039-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca039-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca039-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca039-116">Not supported.</span></span>|
|<span data-ttu-id="ca039-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca039-117">Application</span></span>|<span data-ttu-id="ca039-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca039-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca039-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca039-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca039-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ca039-120">Optional query parameters</span></span>
<span data-ttu-id="ca039-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ca039-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ca039-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca039-122">Request headers</span></span>
|<span data-ttu-id="ca039-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca039-123">Header</span></span>|<span data-ttu-id="ca039-124">値</span><span class="sxs-lookup"><span data-stu-id="ca039-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca039-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca039-125">Authorization</span></span>|<span data-ttu-id="ca039-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ca039-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca039-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ca039-127">Accept</span></span>|<span data-ttu-id="ca039-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ca039-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca039-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca039-129">Request body</span></span>
<span data-ttu-id="ca039-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ca039-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca039-131">応答</span><span class="sxs-lookup"><span data-stu-id="ca039-131">Response</span></span>
<span data-ttu-id="ca039-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ca039-132">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca039-133">例</span><span class="sxs-lookup"><span data-stu-id="ca039-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca039-134">要求</span><span class="sxs-lookup"><span data-stu-id="ca039-134">Request</span></span>
<span data-ttu-id="ca039-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca039-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="ca039-136">応答</span><span class="sxs-lookup"><span data-stu-id="ca039-136">Response</span></span>
<span data-ttu-id="ca039-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca039-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 583

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
    "id": "77943c10-3c10-7794-103c-9477103c9477",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "userId": "User Id value",
    "applicationId": "Application Id value",
    "history": [
      {
        "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
        "occurrenceDateTime": "2017-01-01T00:03:20.8380798-08:00"
      }
    ]
  }
}
```





