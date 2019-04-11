---
title: userPFXCertificate を取得する
description: userPFXCertificate オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 339f7662beae46c2c8513a59bd84c6b66d06a256
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787667"
---
# <a name="get-userpfxcertificate"></a><span data-ttu-id="1eb95-103">userPFXCertificate を取得する</span><span class="sxs-lookup"><span data-stu-id="1eb95-103">Get userPFXCertificate</span></span>

> <span data-ttu-id="1eb95-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1eb95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1eb95-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1eb95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eb95-106">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1eb95-106">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1eb95-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1eb95-107">Prerequisites</span></span>
<span data-ttu-id="1eb95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1eb95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eb95-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1eb95-110">Permission type</span></span>|<span data-ttu-id="1eb95-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1eb95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1eb95-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1eb95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1eb95-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1eb95-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1eb95-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1eb95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1eb95-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1eb95-115">Not supported.</span></span>|
|<span data-ttu-id="1eb95-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1eb95-116">Application</span></span>|<span data-ttu-id="1eb95-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1eb95-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1eb95-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1eb95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1eb95-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1eb95-119">Optional query parameters</span></span>
<span data-ttu-id="1eb95-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1eb95-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1eb95-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1eb95-121">Request headers</span></span>
|<span data-ttu-id="1eb95-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1eb95-122">Header</span></span>|<span data-ttu-id="1eb95-123">値</span><span class="sxs-lookup"><span data-stu-id="1eb95-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1eb95-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1eb95-124">Authorization</span></span>|<span data-ttu-id="1eb95-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1eb95-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1eb95-126">承諾</span><span class="sxs-lookup"><span data-stu-id="1eb95-126">Accept</span></span>|<span data-ttu-id="1eb95-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1eb95-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eb95-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1eb95-128">Request body</span></span>
<span data-ttu-id="1eb95-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1eb95-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1eb95-130">応答</span><span class="sxs-lookup"><span data-stu-id="1eb95-130">Response</span></span>
<span data-ttu-id="1eb95-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1eb95-131">If successful, this method returns a `200 OK` response code and [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1eb95-132">例</span><span class="sxs-lookup"><span data-stu-id="1eb95-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1eb95-133">要求</span><span class="sxs-lookup"><span data-stu-id="1eb95-133">Request</span></span>
<span data-ttu-id="1eb95-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1eb95-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a><span data-ttu-id="1eb95-135">応答</span><span class="sxs-lookup"><span data-stu-id="1eb95-135">Response</span></span>
<span data-ttu-id="1eb95-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1eb95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "value": {
    "@odata.type": "#microsoft.graph.userPFXCertificate",
    "id": "045c159b-159b-045c-9b15-5c049b155c04",
    "thumbprint": "Thumbprint value",
    "intendedPurpose": "smimeEncryption",
    "userPrincipalName": "User Principal Name value",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "providerName": "Provider Name value",
    "keyName": "Key Name value",
    "paddingScheme": "pkcs1",
    "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
    "encryptedPfxPassword": "Encrypted Pfx Password value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```



