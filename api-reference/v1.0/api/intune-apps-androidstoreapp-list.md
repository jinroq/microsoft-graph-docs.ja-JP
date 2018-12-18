---
title: androidStoreApps のリスト
description: androidStoreApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 78897f4663fd79d1a7c4209239b7807e011cfeb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323514"
---
# <a name="list-androidstoreapps"></a><span data-ttu-id="faead-103">androidStoreApps のリスト</span><span class="sxs-lookup"><span data-stu-id="faead-103">List androidStoreApps</span></span>

> <span data-ttu-id="faead-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="faead-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="faead-105">[androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="faead-105">List properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="faead-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="faead-106">Prerequisites</span></span>
<span data-ttu-id="faead-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="faead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faead-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="faead-109">Permission type</span></span>|<span data-ttu-id="faead-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="faead-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faead-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="faead-111">Delegated (work or school account)</span></span>|<span data-ttu-id="faead-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="faead-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="faead-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="faead-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faead-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faead-114">Not supported.</span></span>|
|<span data-ttu-id="faead-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="faead-115">Application</span></span>|<span data-ttu-id="faead-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faead-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faead-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="faead-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="faead-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="faead-118">Request headers</span></span>
|<span data-ttu-id="faead-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="faead-119">Header</span></span>|<span data-ttu-id="faead-120">値</span><span class="sxs-lookup"><span data-stu-id="faead-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faead-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="faead-121">Authorization</span></span>|<span data-ttu-id="faead-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="faead-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faead-123">Accept</span><span class="sxs-lookup"><span data-stu-id="faead-123">Accept</span></span>|<span data-ttu-id="faead-124">application/json</span><span class="sxs-lookup"><span data-stu-id="faead-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faead-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="faead-125">Request body</span></span>
<span data-ttu-id="faead-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="faead-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faead-127">応答</span><span class="sxs-lookup"><span data-stu-id="faead-127">Response</span></span>
<span data-ttu-id="faead-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="faead-128">If successful, this method returns a `200 OK` response code and a collection of [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faead-129">例</span><span class="sxs-lookup"><span data-stu-id="faead-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="faead-130">要求</span><span class="sxs-lookup"><span data-stu-id="faead-130">Request</span></span>
<span data-ttu-id="faead-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="faead-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="faead-132">応答</span><span class="sxs-lookup"><span data-stu-id="faead-132">Response</span></span>
<span data-ttu-id="faead-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="faead-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidStoreApp",
      "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
      "packageId": "Package Id value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
        "v4_0": true,
        "v4_0_3": true,
        "v4_1": true,
        "v4_2": true,
        "v4_3": true,
        "v4_4": true,
        "v5_0": true,
        "v5_1": true
      }
    }
  ]
}
```



