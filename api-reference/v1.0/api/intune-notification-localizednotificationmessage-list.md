---
title: localizedNotificationMessages のリスト
description: localizedNotificationMessage オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 563b324eca95f5b5b26eaeb00d192467055cb13b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252232"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="b75c0-103">localizedNotificationMessages のリスト</span><span class="sxs-lookup"><span data-stu-id="b75c0-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="b75c0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b75c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b75c0-105">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b75c0-105">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b75c0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b75c0-106">Prerequisites</span></span>
<span data-ttu-id="b75c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b75c0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b75c0-109">Permission type</span></span>|<span data-ttu-id="b75c0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b75c0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b75c0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b75c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b75c0-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b75c0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b75c0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b75c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b75c0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b75c0-114">Not supported.</span></span>|
|<span data-ttu-id="b75c0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b75c0-115">Application</span></span>|<span data-ttu-id="b75c0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b75c0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b75c0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b75c0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="b75c0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b75c0-118">Request headers</span></span>
|<span data-ttu-id="b75c0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b75c0-119">Header</span></span>|<span data-ttu-id="b75c0-120">値</span><span class="sxs-lookup"><span data-stu-id="b75c0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b75c0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b75c0-121">Authorization</span></span>|<span data-ttu-id="b75c0-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b75c0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b75c0-123">承諾</span><span class="sxs-lookup"><span data-stu-id="b75c0-123">Accept</span></span>|<span data-ttu-id="b75c0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b75c0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b75c0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b75c0-125">Request body</span></span>
<span data-ttu-id="b75c0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b75c0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b75c0-127">応答</span><span class="sxs-lookup"><span data-stu-id="b75c0-127">Response</span></span>
<span data-ttu-id="b75c0-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b75c0-128">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b75c0-129">例</span><span class="sxs-lookup"><span data-stu-id="b75c0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b75c0-130">要求</span><span class="sxs-lookup"><span data-stu-id="b75c0-130">Request</span></span>
<span data-ttu-id="b75c0-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b75c0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="b75c0-132">応答</span><span class="sxs-lookup"><span data-stu-id="b75c0-132">Response</span></span>
<span data-ttu-id="b75c0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b75c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



