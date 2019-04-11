---
title: リスト userPFXCertificates
description: userPFXCertificate オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d885555158c8caf83fee11e51f29ea2433e76797
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790355"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="de675-103">リスト userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="de675-103">List userPFXCertificates</span></span>

> <span data-ttu-id="de675-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de675-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de675-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="de675-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de675-106">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="de675-106">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de675-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="de675-107">Prerequisites</span></span>
<span data-ttu-id="de675-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de675-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de675-110">Permission type</span></span>|<span data-ttu-id="de675-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="de675-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de675-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de675-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de675-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="de675-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="de675-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de675-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de675-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de675-115">Not supported.</span></span>|
|<span data-ttu-id="de675-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de675-116">Application</span></span>|<span data-ttu-id="de675-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de675-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de675-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de675-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="de675-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de675-119">Request headers</span></span>
|<span data-ttu-id="de675-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de675-120">Header</span></span>|<span data-ttu-id="de675-121">値</span><span class="sxs-lookup"><span data-stu-id="de675-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de675-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de675-122">Authorization</span></span>|<span data-ttu-id="de675-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="de675-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de675-124">承諾</span><span class="sxs-lookup"><span data-stu-id="de675-124">Accept</span></span>|<span data-ttu-id="de675-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de675-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de675-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="de675-126">Request body</span></span>
<span data-ttu-id="de675-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="de675-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de675-128">応答</span><span class="sxs-lookup"><span data-stu-id="de675-128">Response</span></span>
<span data-ttu-id="de675-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="de675-129">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de675-130">例</span><span class="sxs-lookup"><span data-stu-id="de675-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="de675-131">要求</span><span class="sxs-lookup"><span data-stu-id="de675-131">Request</span></span>
<span data-ttu-id="de675-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de675-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="de675-133">応答</span><span class="sxs-lookup"><span data-stu-id="de675-133">Response</span></span>
<span data-ttu-id="de675-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de675-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 784

{
  "value": [
    {
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
  ]
}
```



