---
title: リスト mobileAppTroubleshootingEvents
description: MobileAppTroubleshootingEvent オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a4185a9ae976bf944c90bb8687d8b8d56c085d9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851885"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="f1931-103">リスト mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="f1931-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="f1931-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f1931-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1931-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1931-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1931-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1931-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1931-107">[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f1931-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1931-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f1931-108">Prerequisites</span></span>
<span data-ttu-id="f1931-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1931-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1931-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1931-111">Permission type</span></span>|<span data-ttu-id="f1931-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1931-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1931-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1931-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1931-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1931-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f1931-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1931-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1931-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1931-116">Not supported.</span></span>|
|<span data-ttu-id="f1931-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1931-117">Application</span></span>|<span data-ttu-id="f1931-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1931-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1931-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1931-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f1931-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1931-120">Request headers</span></span>
|<span data-ttu-id="f1931-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1931-121">Header</span></span>|<span data-ttu-id="f1931-122">値</span><span class="sxs-lookup"><span data-stu-id="f1931-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1931-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1931-123">Authorization</span></span>|<span data-ttu-id="f1931-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f1931-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1931-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1931-125">Accept</span></span>|<span data-ttu-id="f1931-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1931-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1931-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1931-127">Request body</span></span>
<span data-ttu-id="f1931-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1931-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1931-129">応答</span><span class="sxs-lookup"><span data-stu-id="f1931-129">Response</span></span>
<span data-ttu-id="f1931-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f1931-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1931-131">例</span><span class="sxs-lookup"><span data-stu-id="f1931-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1931-132">要求</span><span class="sxs-lookup"><span data-stu-id="f1931-132">Request</span></span>
<span data-ttu-id="f1931-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1931-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="f1931-134">応答</span><span class="sxs-lookup"><span data-stu-id="f1931-134">Response</span></span>
<span data-ttu-id="f1931-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1931-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 623

{
  "value": [
    {
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
  ]
}
```





