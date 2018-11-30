---
title: Get iosVppEBook
description: iosVppEBook オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: fd30838d4779813c3b9fe98ea11414b5f8bbaf06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023460"
---
# <a name="get-iosvppebook"></a><span data-ttu-id="1add8-103">Get iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="1add8-103">Get iosVppEBook</span></span>

> <span data-ttu-id="1add8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1add8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1add8-105">[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1add8-105">Read properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1add8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1add8-106">Prerequisites</span></span>
<span data-ttu-id="1add8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1add8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1add8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1add8-109">Permission type</span></span>|<span data-ttu-id="1add8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1add8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1add8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1add8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1add8-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1add8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1add8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1add8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1add8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1add8-114">Not supported.</span></span>|
|<span data-ttu-id="1add8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1add8-115">Application</span></span>|<span data-ttu-id="1add8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1add8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1add8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1add8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1add8-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1add8-118">Optional query parameters</span></span>
<span data-ttu-id="1add8-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1add8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1add8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1add8-120">Request headers</span></span>
|<span data-ttu-id="1add8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1add8-121">Header</span></span>|<span data-ttu-id="1add8-122">値</span><span class="sxs-lookup"><span data-stu-id="1add8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1add8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1add8-123">Authorization</span></span>|<span data-ttu-id="1add8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1add8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1add8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1add8-125">Accept</span></span>|<span data-ttu-id="1add8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1add8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1add8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1add8-127">Request body</span></span>
<span data-ttu-id="1add8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1add8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1add8-129">応答</span><span class="sxs-lookup"><span data-stu-id="1add8-129">Response</span></span>
<span data-ttu-id="1add8-130">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1add8-130">If successful, this method returns a `200 OK` response code and [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1add8-131">例</span><span class="sxs-lookup"><span data-stu-id="1add8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1add8-132">要求</span><span class="sxs-lookup"><span data-stu-id="1add8-132">Request</span></span>
<span data-ttu-id="1add8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1add8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="1add8-134">応答</span><span class="sxs-lookup"><span data-stu-id="1add8-134">Response</span></span>
<span data-ttu-id="1add8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1add8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1033

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppEBook",
    "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
    "largeCover": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "informationUrl": "https://example.com/informationUrl/",
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
    "appleId": "Apple Id value",
    "vppOrganizationName": "Vpp Organization Name value",
    "genres": [
      "Genres value"
    ],
    "language": "Language value",
    "seller": "Seller value",
    "totalLicenseCount": 1,
    "usedLicenseCount": 0
  }
}
```



