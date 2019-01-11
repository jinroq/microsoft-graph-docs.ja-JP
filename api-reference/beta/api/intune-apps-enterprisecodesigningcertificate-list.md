---
title: リスト enterpriseCodeSigningCertificates
description: EnterpriseCodeSigningCertificate オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 648b58e12ebd314366ff171ee5a4304b8aac59bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824434"
---
# <a name="list-enterprisecodesigningcertificates"></a><span data-ttu-id="b6824-103">リスト enterpriseCodeSigningCertificates</span><span class="sxs-lookup"><span data-stu-id="b6824-103">List enterpriseCodeSigningCertificates</span></span>

> <span data-ttu-id="b6824-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b6824-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6824-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6824-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6824-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6824-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6824-107">[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b6824-107">List properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6824-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6824-108">Prerequisites</span></span>
<span data-ttu-id="b6824-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6824-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6824-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6824-111">Permission type</span></span>|<span data-ttu-id="b6824-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6824-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6824-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6824-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6824-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6824-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b6824-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6824-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6824-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6824-116">Not supported.</span></span>|
|<span data-ttu-id="b6824-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6824-117">Application</span></span>|<span data-ttu-id="b6824-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6824-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6824-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6824-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="b6824-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6824-120">Request headers</span></span>
|<span data-ttu-id="b6824-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6824-121">Header</span></span>|<span data-ttu-id="b6824-122">値</span><span class="sxs-lookup"><span data-stu-id="b6824-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6824-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6824-123">Authorization</span></span>|<span data-ttu-id="b6824-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b6824-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6824-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6824-125">Accept</span></span>|<span data-ttu-id="b6824-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6824-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6824-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6824-127">Request body</span></span>
<span data-ttu-id="b6824-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6824-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6824-129">応答</span><span class="sxs-lookup"><span data-stu-id="b6824-129">Response</span></span>
<span data-ttu-id="b6824-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b6824-130">If successful, this method returns a `200 OK` response code and a collection of [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6824-131">例</span><span class="sxs-lookup"><span data-stu-id="b6824-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6824-132">要求</span><span class="sxs-lookup"><span data-stu-id="b6824-132">Request</span></span>
<span data-ttu-id="b6824-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6824-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
```

### <a name="response"></a><span data-ttu-id="b6824-134">応答</span><span class="sxs-lookup"><span data-stu-id="b6824-134">Response</span></span>
<span data-ttu-id="b6824-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6824-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
      "id": "b20d3703-3703-b20d-0337-0db203370db2",
      "content": "Y29udGVudA==",
      "status": "provisioned",
      "subjectName": "Subject Name value",
      "subject": "Subject value",
      "issuerName": "Issuer Name value",
      "issuer": "Issuer value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
    }
  ]
}
```





