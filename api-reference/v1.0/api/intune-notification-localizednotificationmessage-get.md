---
title: localizedNotificationMessage の取得
description: localizedNotificationMessage オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18ee8e6cafd441344362055f0e5c4463b38454bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974788"
---
# <a name="get-localizednotificationmessage"></a><span data-ttu-id="6dca1-103">localizedNotificationMessage の取得</span><span class="sxs-lookup"><span data-stu-id="6dca1-103">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="6dca1-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dca1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dca1-105">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6dca1-105">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dca1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6dca1-106">Prerequisites</span></span>
<span data-ttu-id="6dca1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6dca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dca1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6dca1-109">Permission type</span></span>|<span data-ttu-id="6dca1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6dca1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dca1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6dca1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dca1-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dca1-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6dca1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6dca1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dca1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dca1-114">Not supported.</span></span>|
|<span data-ttu-id="6dca1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6dca1-115">Application</span></span>|<span data-ttu-id="6dca1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dca1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dca1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6dca1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dca1-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6dca1-118">Optional query parameters</span></span>
<span data-ttu-id="6dca1-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6dca1-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dca1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dca1-120">Request headers</span></span>
|<span data-ttu-id="6dca1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dca1-121">Header</span></span>|<span data-ttu-id="6dca1-122">値</span><span class="sxs-lookup"><span data-stu-id="6dca1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dca1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dca1-123">Authorization</span></span>|<span data-ttu-id="6dca1-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dca1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dca1-125">承諾</span><span class="sxs-lookup"><span data-stu-id="6dca1-125">Accept</span></span>|<span data-ttu-id="6dca1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6dca1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dca1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6dca1-127">Request body</span></span>
<span data-ttu-id="6dca1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6dca1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dca1-129">応答</span><span class="sxs-lookup"><span data-stu-id="6dca1-129">Response</span></span>
<span data-ttu-id="6dca1-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6dca1-130">If successful, this method returns a `200 OK` response code and [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dca1-131">例</span><span class="sxs-lookup"><span data-stu-id="6dca1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dca1-132">要求</span><span class="sxs-lookup"><span data-stu-id="6dca1-132">Request</span></span>
<span data-ttu-id="6dca1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6dca1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="6dca1-134">応答</span><span class="sxs-lookup"><span data-stu-id="6dca1-134">Response</span></span>
<span data-ttu-id="6dca1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6dca1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.localizedNotificationMessage",
    "id": "7a777708-7708-7a77-0877-777a0877777a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "locale": "Locale value",
    "subject": "Subject value",
    "messageTemplate": "Message Template value",
    "isDefault": true
  }
}
```



