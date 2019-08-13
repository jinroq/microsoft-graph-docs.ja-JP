---
title: localizedNotificationMessages のリスト
description: localizedNotificationMessage オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a0d4d595886e57983ca10fd046d4459c0f76ee8a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353289"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="f319e-103">localizedNotificationMessages のリスト</span><span class="sxs-lookup"><span data-stu-id="f319e-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="f319e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f319e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f319e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f319e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f319e-106">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f319e-106">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f319e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f319e-107">Prerequisites</span></span>
<span data-ttu-id="f319e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f319e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f319e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f319e-110">Permission type</span></span>|<span data-ttu-id="f319e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f319e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f319e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f319e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f319e-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f319e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f319e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f319e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f319e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f319e-115">Not supported.</span></span>|
|<span data-ttu-id="f319e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f319e-116">Application</span></span>|<span data-ttu-id="f319e-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f319e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f319e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f319e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="f319e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f319e-119">Request headers</span></span>
|<span data-ttu-id="f319e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f319e-120">Header</span></span>|<span data-ttu-id="f319e-121">値</span><span class="sxs-lookup"><span data-stu-id="f319e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f319e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f319e-122">Authorization</span></span>|<span data-ttu-id="f319e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f319e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f319e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f319e-124">Accept</span></span>|<span data-ttu-id="f319e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f319e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f319e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f319e-126">Request body</span></span>
<span data-ttu-id="f319e-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f319e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f319e-128">応答</span><span class="sxs-lookup"><span data-stu-id="f319e-128">Response</span></span>
<span data-ttu-id="f319e-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f319e-129">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f319e-130">例</span><span class="sxs-lookup"><span data-stu-id="f319e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f319e-131">要求</span><span class="sxs-lookup"><span data-stu-id="f319e-131">Request</span></span>
<span data-ttu-id="f319e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f319e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="f319e-133">応答</span><span class="sxs-lookup"><span data-stu-id="f319e-133">Response</span></span>
<span data-ttu-id="f319e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f319e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.localizedNotificationMessage",
      "id": "7a777708-7708-7a77-0877-777a0877777a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "locale": "Locale value",
      "subject": "Subject value",
      "messageTemplate": "Message Template value",
      "isDefault": true
    }
  ]
}
```






