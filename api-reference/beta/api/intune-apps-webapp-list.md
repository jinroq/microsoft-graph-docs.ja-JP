---
title: webApps のリスト
description: webApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 08a1ced13d785e1a33b4b719aecb9b5b6947f0c8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337927"
---
# <a name="list-webapps"></a><span data-ttu-id="252fe-103">webApps のリスト</span><span class="sxs-lookup"><span data-stu-id="252fe-103">List webApps</span></span>

> <span data-ttu-id="252fe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="252fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="252fe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="252fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="252fe-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="252fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="252fe-107">[webApp](../resources/intune-apps-webapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="252fe-107">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="252fe-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="252fe-108">Prerequisites</span></span>
<span data-ttu-id="252fe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="252fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="252fe-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="252fe-111">Permission type</span></span>|<span data-ttu-id="252fe-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="252fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="252fe-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="252fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="252fe-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="252fe-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="252fe-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="252fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="252fe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="252fe-116">Not supported.</span></span>|
|<span data-ttu-id="252fe-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="252fe-117">Application</span></span>|<span data-ttu-id="252fe-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="252fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="252fe-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="252fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="252fe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="252fe-120">Request headers</span></span>
|<span data-ttu-id="252fe-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="252fe-121">Header</span></span>|<span data-ttu-id="252fe-122">値</span><span class="sxs-lookup"><span data-stu-id="252fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="252fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="252fe-123">Authorization</span></span>|<span data-ttu-id="252fe-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="252fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="252fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="252fe-125">Accept</span></span>|<span data-ttu-id="252fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="252fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="252fe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="252fe-127">Request body</span></span>
<span data-ttu-id="252fe-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="252fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="252fe-129">応答</span><span class="sxs-lookup"><span data-stu-id="252fe-129">Response</span></span>
<span data-ttu-id="252fe-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [webApp](../resources/intune-apps-webapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="252fe-130">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="252fe-131">例</span><span class="sxs-lookup"><span data-stu-id="252fe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="252fe-132">要求</span><span class="sxs-lookup"><span data-stu-id="252fe-132">Request</span></span>
<span data-ttu-id="252fe-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="252fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="252fe-134">応答</span><span class="sxs-lookup"><span data-stu-id="252fe-134">Response</span></span>
<span data-ttu-id="252fe-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="252fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 960

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.webApp",
      "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
      "uploadState": 11,
      "publishingState": "processing",
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```




