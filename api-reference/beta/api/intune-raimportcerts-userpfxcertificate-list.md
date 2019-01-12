---
title: リスト userPFXCertificates
description: UserPFXCertificate オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2f186842a5dc22a6fd43472b421988e4babb1fb9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940331"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="edcfd-103">リスト userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="edcfd-103">List userPFXCertificates</span></span>

> <span data-ttu-id="edcfd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="edcfd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edcfd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="edcfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="edcfd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="edcfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edcfd-107">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="edcfd-107">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edcfd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="edcfd-108">Prerequisites</span></span>
<span data-ttu-id="edcfd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="edcfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edcfd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="edcfd-111">Permission type</span></span>|<span data-ttu-id="edcfd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="edcfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edcfd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="edcfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edcfd-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="edcfd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="edcfd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="edcfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edcfd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="edcfd-116">Not supported.</span></span>|
|<span data-ttu-id="edcfd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="edcfd-117">Application</span></span>|<span data-ttu-id="edcfd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="edcfd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edcfd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="edcfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="edcfd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="edcfd-120">Request headers</span></span>
|<span data-ttu-id="edcfd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="edcfd-121">Header</span></span>|<span data-ttu-id="edcfd-122">値</span><span class="sxs-lookup"><span data-stu-id="edcfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edcfd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="edcfd-123">Authorization</span></span>|<span data-ttu-id="edcfd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="edcfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edcfd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="edcfd-125">Accept</span></span>|<span data-ttu-id="edcfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edcfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edcfd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="edcfd-127">Request body</span></span>
<span data-ttu-id="edcfd-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="edcfd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edcfd-129">応答</span><span class="sxs-lookup"><span data-stu-id="edcfd-129">Response</span></span>
<span data-ttu-id="edcfd-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="edcfd-130">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edcfd-131">例</span><span class="sxs-lookup"><span data-stu-id="edcfd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="edcfd-132">要求</span><span class="sxs-lookup"><span data-stu-id="edcfd-132">Request</span></span>
<span data-ttu-id="edcfd-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="edcfd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="edcfd-134">応答</span><span class="sxs-lookup"><span data-stu-id="edcfd-134">Response</span></span>
<span data-ttu-id="edcfd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="edcfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





