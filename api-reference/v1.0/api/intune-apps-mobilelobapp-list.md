---
title: mobileLobApps のリスト
description: mobileLobApp オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 370fdf99a3506aa97b10ee1546af2f0b3acc0733
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023083"
---
# <a name="list-mobilelobapps"></a><span data-ttu-id="cdabe-103">mobileLobApps のリスト</span><span class="sxs-lookup"><span data-stu-id="cdabe-103">List mobileLobApps</span></span>

> <span data-ttu-id="cdabe-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cdabe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdabe-105">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cdabe-105">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdabe-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cdabe-106">Prerequisites</span></span>
<span data-ttu-id="cdabe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdabe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdabe-109">Permission type</span></span>|<span data-ttu-id="cdabe-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdabe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdabe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdabe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdabe-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdabe-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cdabe-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdabe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdabe-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdabe-114">Not supported.</span></span>|
|<span data-ttu-id="cdabe-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdabe-115">Application</span></span>|<span data-ttu-id="cdabe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdabe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdabe-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdabe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cdabe-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdabe-118">Request headers</span></span>
|<span data-ttu-id="cdabe-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdabe-119">Header</span></span>|<span data-ttu-id="cdabe-120">値</span><span class="sxs-lookup"><span data-stu-id="cdabe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdabe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdabe-121">Authorization</span></span>|<span data-ttu-id="cdabe-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cdabe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdabe-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cdabe-123">Accept</span></span>|<span data-ttu-id="cdabe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cdabe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdabe-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cdabe-125">Request body</span></span>
<span data-ttu-id="cdabe-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cdabe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdabe-127">応答</span><span class="sxs-lookup"><span data-stu-id="cdabe-127">Response</span></span>
<span data-ttu-id="cdabe-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cdabe-128">If successful, this method returns a `200 OK` response code and a collection of [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdabe-129">例</span><span class="sxs-lookup"><span data-stu-id="cdabe-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdabe-130">要求</span><span class="sxs-lookup"><span data-stu-id="cdabe-130">Request</span></span>
<span data-ttu-id="cdabe-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cdabe-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="cdabe-132">応答</span><span class="sxs-lookup"><span data-stu-id="cdabe-132">Response</span></span>
<span data-ttu-id="cdabe-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cdabe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 983

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileLobApp",
      "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
      "size": 4
    }
  ]
}
```


