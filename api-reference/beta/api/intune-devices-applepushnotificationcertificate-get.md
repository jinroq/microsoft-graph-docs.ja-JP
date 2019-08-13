---
title: applePushNotificationCertificate の取得
description: applePushNotificationCertificate オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89ab84dc42bc685d1e8787c43dad9958dcd732d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348936"
---
# <a name="get-applepushnotificationcertificate"></a><span data-ttu-id="fdabc-103">applePushNotificationCertificate の取得</span><span class="sxs-lookup"><span data-stu-id="fdabc-103">Get applePushNotificationCertificate</span></span>

> <span data-ttu-id="fdabc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fdabc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdabc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fdabc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdabc-106">[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fdabc-106">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdabc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fdabc-107">Prerequisites</span></span>
<span data-ttu-id="fdabc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fdabc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdabc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fdabc-110">Permission type</span></span>|<span data-ttu-id="fdabc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fdabc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdabc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fdabc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fdabc-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdabc-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fdabc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fdabc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdabc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fdabc-115">Not supported.</span></span>|
|<span data-ttu-id="fdabc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fdabc-116">Application</span></span>|<span data-ttu-id="fdabc-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdabc-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdabc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fdabc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/applePushNotificationCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdabc-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fdabc-119">Optional query parameters</span></span>
<span data-ttu-id="fdabc-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fdabc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdabc-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fdabc-121">Request headers</span></span>
|<span data-ttu-id="fdabc-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fdabc-122">Header</span></span>|<span data-ttu-id="fdabc-123">値</span><span class="sxs-lookup"><span data-stu-id="fdabc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdabc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdabc-124">Authorization</span></span>|<span data-ttu-id="fdabc-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fdabc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdabc-126">承諾</span><span class="sxs-lookup"><span data-stu-id="fdabc-126">Accept</span></span>|<span data-ttu-id="fdabc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fdabc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdabc-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fdabc-128">Request body</span></span>
<span data-ttu-id="fdabc-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fdabc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdabc-130">応答</span><span class="sxs-lookup"><span data-stu-id="fdabc-130">Response</span></span>
<span data-ttu-id="fdabc-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fdabc-131">If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdabc-132">例</span><span class="sxs-lookup"><span data-stu-id="fdabc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdabc-133">要求</span><span class="sxs-lookup"><span data-stu-id="fdabc-133">Request</span></span>
<span data-ttu-id="fdabc-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fdabc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### <a name="response"></a><span data-ttu-id="fdabc-135">応答</span><span class="sxs-lookup"><span data-stu-id="fdabc-135">Response</span></span>
<span data-ttu-id="fdabc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fdabc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificateUploadStatus": "Certificate Upload Status value",
    "certificateUploadFailureReason": "Certificate Upload Failure Reason value",
    "certificate": "Certificate value"
  }
}
```






