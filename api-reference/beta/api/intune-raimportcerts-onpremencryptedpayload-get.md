---
title: OnPremEncryptedPayload を取得する
description: OnPremEncryptedPayload オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ea86f77bb29418f3acb8f79afc65ec5eccba13b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741459"
---
# <a name="get-onpremencryptedpayload"></a><span data-ttu-id="f36f3-103">OnPremEncryptedPayload を取得する</span><span class="sxs-lookup"><span data-stu-id="f36f3-103">Get onPremEncryptedPayload</span></span>

> <span data-ttu-id="f36f3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f36f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f36f3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f36f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f36f3-106">[OnPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f36f3-106">Read properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f36f3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f36f3-107">Prerequisites</span></span>
<span data-ttu-id="f36f3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f36f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f36f3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f36f3-110">Permission type</span></span>|<span data-ttu-id="f36f3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f36f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f36f3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f36f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f36f3-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f36f3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f36f3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f36f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f36f3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f36f3-115">Not supported.</span></span>|
|<span data-ttu-id="f36f3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f36f3-116">Application</span></span>|<span data-ttu-id="f36f3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f36f3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f36f3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f36f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f36f3-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f36f3-119">Optional query parameters</span></span>
<span data-ttu-id="f36f3-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f36f3-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f36f3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f36f3-121">Request headers</span></span>
|<span data-ttu-id="f36f3-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f36f3-122">Header</span></span>|<span data-ttu-id="f36f3-123">値</span><span class="sxs-lookup"><span data-stu-id="f36f3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f36f3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f36f3-124">Authorization</span></span>|<span data-ttu-id="f36f3-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f36f3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f36f3-126">承諾</span><span class="sxs-lookup"><span data-stu-id="f36f3-126">Accept</span></span>|<span data-ttu-id="f36f3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f36f3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f36f3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f36f3-128">Request body</span></span>
<span data-ttu-id="f36f3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f36f3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f36f3-130">応答</span><span class="sxs-lookup"><span data-stu-id="f36f3-130">Response</span></span>
<span data-ttu-id="f36f3-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f36f3-131">If successful, this method returns a `200 OK` response code and [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f36f3-132">例</span><span class="sxs-lookup"><span data-stu-id="f36f3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f36f3-133">要求</span><span class="sxs-lookup"><span data-stu-id="f36f3-133">Request</span></span>
<span data-ttu-id="f36f3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f36f3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

### <a name="response"></a><span data-ttu-id="f36f3-135">応答</span><span class="sxs-lookup"><span data-stu-id="f36f3-135">Response</span></span>
<span data-ttu-id="f36f3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f36f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
    "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
    "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
    "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
    "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
    "deviceKeyThumbprint": "Device Key Thumbprint value",
    "cert1PayloadUUID": "Cert1Payload UUID value",
    "cert2PayloadUUID": "Cert2Payload UUID value",
    "cert3PayloadUUID": "Cert3Payload UUID value",
    "plistTemplate": "Plist Template value",
    "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
    "payloadVersion": 14,
    "status": 6,
    "createdTime": "2017-01-01T00:03:18.9597073-08:00",
    "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
    "eTag": "ETag value",
    "isDeleted": true
  }
}
```




