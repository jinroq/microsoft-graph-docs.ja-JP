---
title: windowsMobileMSIs のリスト
description: windowsMobileMSI オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 4ca60c76978812333981aaefc93f6e10a901904b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349967"
---
# <a name="list-windowsmobilemsis"></a><span data-ttu-id="8296a-103">windowsMobileMSIs のリスト</span><span class="sxs-lookup"><span data-stu-id="8296a-103">List windowsMobileMSIs</span></span>

> <span data-ttu-id="8296a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8296a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8296a-105">[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8296a-105">List properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8296a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8296a-106">Prerequisites</span></span>
<span data-ttu-id="8296a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8296a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8296a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8296a-109">Permission type</span></span>|<span data-ttu-id="8296a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8296a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8296a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8296a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8296a-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8296a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8296a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8296a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8296a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8296a-114">Not supported.</span></span>|
|<span data-ttu-id="8296a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8296a-115">Application</span></span>|<span data-ttu-id="8296a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8296a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8296a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8296a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8296a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8296a-118">Request headers</span></span>
|<span data-ttu-id="8296a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8296a-119">Header</span></span>|<span data-ttu-id="8296a-120">値</span><span class="sxs-lookup"><span data-stu-id="8296a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8296a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8296a-121">Authorization</span></span>|<span data-ttu-id="8296a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8296a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8296a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8296a-123">Accept</span></span>|<span data-ttu-id="8296a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8296a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8296a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8296a-125">Request body</span></span>
<span data-ttu-id="8296a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8296a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8296a-127">応答</span><span class="sxs-lookup"><span data-stu-id="8296a-127">Response</span></span>
<span data-ttu-id="8296a-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8296a-128">If successful, this method returns a `200 OK` response code and a collection of [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8296a-129">例</span><span class="sxs-lookup"><span data-stu-id="8296a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8296a-130">要求</span><span class="sxs-lookup"><span data-stu-id="8296a-130">Request</span></span>
<span data-ttu-id="8296a-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8296a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="8296a-132">応答</span><span class="sxs-lookup"><span data-stu-id="8296a-132">Response</span></span>
<span data-ttu-id="8296a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8296a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1164

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsMobileMSI",
      "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "publishingState": "processing",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "commandLine": "Command Line value",
      "productCode": "Product Code value",
      "productVersion": "Product Version value",
      "ignoreVersionDetection": true
    }
  ]
}
```


