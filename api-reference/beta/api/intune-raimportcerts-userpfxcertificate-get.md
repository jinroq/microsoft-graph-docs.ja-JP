---
title: UserPFXCertificate を取得する
description: UserPFXCertificate オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90f105caa1edfb30b23cb7a690f6a2c5c93dfc5d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993810"
---
# <a name="get-userpfxcertificate"></a><span data-ttu-id="e9950-103">UserPFXCertificate を取得する</span><span class="sxs-lookup"><span data-stu-id="e9950-103">Get userPFXCertificate</span></span>

> <span data-ttu-id="e9950-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9950-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9950-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9950-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9950-106">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e9950-106">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9950-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e9950-107">Prerequisites</span></span>
<span data-ttu-id="e9950-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9950-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e9950-110">Permission type</span></span>|<span data-ttu-id="e9950-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e9950-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9950-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e9950-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9950-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9950-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e9950-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e9950-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9950-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9950-115">Not supported.</span></span>|
|<span data-ttu-id="e9950-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e9950-116">Application</span></span>|<span data-ttu-id="e9950-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9950-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9950-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e9950-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9950-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9950-119">Optional query parameters</span></span>
<span data-ttu-id="e9950-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e9950-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9950-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9950-121">Request headers</span></span>
|<span data-ttu-id="e9950-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9950-122">Header</span></span>|<span data-ttu-id="e9950-123">値</span><span class="sxs-lookup"><span data-stu-id="e9950-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9950-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9950-124">Authorization</span></span>|<span data-ttu-id="e9950-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9950-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9950-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e9950-126">Accept</span></span>|<span data-ttu-id="e9950-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e9950-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9950-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e9950-128">Request body</span></span>
<span data-ttu-id="e9950-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e9950-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9950-130">応答</span><span class="sxs-lookup"><span data-stu-id="e9950-130">Response</span></span>
<span data-ttu-id="e9950-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e9950-131">If successful, this method returns a `200 OK` response code and [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9950-132">例</span><span class="sxs-lookup"><span data-stu-id="e9950-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9950-133">要求</span><span class="sxs-lookup"><span data-stu-id="e9950-133">Request</span></span>
<span data-ttu-id="e9950-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e9950-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a><span data-ttu-id="e9950-135">応答</span><span class="sxs-lookup"><span data-stu-id="e9950-135">Response</span></span>
<span data-ttu-id="e9950-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e9950-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





