---
title: consentToDataSharing アクション
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 2e2e8f198c10e1ff043544ee25dcdb889a9e2635
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329891"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="1d5a0-103">consentToDataSharing アクション</span><span class="sxs-lookup"><span data-stu-id="1d5a0-103">consentToDataSharing action</span></span>

> <span data-ttu-id="1d5a0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d5a0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d5a0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d5a0-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1d5a0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d5a0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1d5a0-108">Prerequisites</span></span>
<span data-ttu-id="1d5a0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d5a0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d5a0-111">Permission type</span></span>|<span data-ttu-id="1d5a0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d5a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d5a0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d5a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d5a0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d5a0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1d5a0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d5a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d5a0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-116">Not supported.</span></span>|
|<span data-ttu-id="1d5a0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d5a0-117">Application</span></span>|<span data-ttu-id="1d5a0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d5a0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d5a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="1d5a0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d5a0-120">Request headers</span></span>
|<span data-ttu-id="1d5a0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d5a0-121">Header</span></span>|<span data-ttu-id="1d5a0-122">値</span><span class="sxs-lookup"><span data-stu-id="1d5a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d5a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d5a0-123">Authorization</span></span>|<span data-ttu-id="1d5a0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d5a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d5a0-125">Accept</span></span>|<span data-ttu-id="1d5a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d5a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d5a0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d5a0-127">Request body</span></span>
<span data-ttu-id="1d5a0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d5a0-129">応答</span><span class="sxs-lookup"><span data-stu-id="1d5a0-129">Response</span></span>
<span data-ttu-id="1d5a0-130">かどうか、成功を返すアクション、`200 OK`応答コードおよび応答の本文には[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)です。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-130">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d5a0-131">例</span><span class="sxs-lookup"><span data-stu-id="1d5a0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d5a0-132">要求</span><span class="sxs-lookup"><span data-stu-id="1d5a0-132">Request</span></span>
<span data-ttu-id="1d5a0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="1d5a0-134">応答</span><span class="sxs-lookup"><span data-stu-id="1d5a0-134">Response</span></span>
<span data-ttu-id="1d5a0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d5a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.dataSharingConsent",
    "id": "333387f7-87f7-3333-f787-3333f7873333",
    "serviceDisplayName": "Service Display Name value",
    "termsUrl": "https://example.com/termsUrl/",
    "granted": true,
    "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
    "grantedByUpn": "Granted By Upn value",
    "grantedByUserId": "Granted By User Id value"
  }
}
```





