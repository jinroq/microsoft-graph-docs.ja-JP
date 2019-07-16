---
title: リスト onPremEncryptedPayloads
description: OnPremEncryptedPayload オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9a236500120e1060d8450db1a5bc5a1d6d8db00
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741458"
---
# <a name="list-onpremencryptedpayloads"></a><span data-ttu-id="60bbc-103">リスト onPremEncryptedPayloads</span><span class="sxs-lookup"><span data-stu-id="60bbc-103">List onPremEncryptedPayloads</span></span>

> <span data-ttu-id="60bbc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60bbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60bbc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="60bbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60bbc-106">[OnPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="60bbc-106">List properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60bbc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="60bbc-107">Prerequisites</span></span>
<span data-ttu-id="60bbc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60bbc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60bbc-110">Permission type</span></span>|<span data-ttu-id="60bbc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="60bbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60bbc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60bbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60bbc-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="60bbc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="60bbc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60bbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60bbc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60bbc-115">Not supported.</span></span>|
|<span data-ttu-id="60bbc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60bbc-116">Application</span></span>|<span data-ttu-id="60bbc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60bbc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60bbc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60bbc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="60bbc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60bbc-119">Request headers</span></span>
|<span data-ttu-id="60bbc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60bbc-120">Header</span></span>|<span data-ttu-id="60bbc-121">値</span><span class="sxs-lookup"><span data-stu-id="60bbc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60bbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60bbc-122">Authorization</span></span>|<span data-ttu-id="60bbc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="60bbc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60bbc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="60bbc-124">Accept</span></span>|<span data-ttu-id="60bbc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60bbc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60bbc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="60bbc-126">Request body</span></span>
<span data-ttu-id="60bbc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="60bbc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60bbc-128">応答</span><span class="sxs-lookup"><span data-stu-id="60bbc-128">Response</span></span>
<span data-ttu-id="60bbc-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="60bbc-129">If successful, this method returns a `200 OK` response code and a collection of [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60bbc-130">例</span><span class="sxs-lookup"><span data-stu-id="60bbc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="60bbc-131">要求</span><span class="sxs-lookup"><span data-stu-id="60bbc-131">Request</span></span>
<span data-ttu-id="60bbc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60bbc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads
```

### <a name="response"></a><span data-ttu-id="60bbc-133">応答</span><span class="sxs-lookup"><span data-stu-id="60bbc-133">Response</span></span>
<span data-ttu-id="60bbc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60bbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 882

{
  "value": [
    {
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
  ]
}
```





