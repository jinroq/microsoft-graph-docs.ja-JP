---
title: microsoftStoreForBusinessApps のリスト
description: microsoftStoreForBusinessApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 979a5ddaf3f7594b6d4ef2b474f873d5f9806506
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894139"
---
# <a name="list-microsoftstoreforbusinessapps"></a><span data-ttu-id="25bbb-103">microsoftStoreForBusinessApps のリスト</span><span class="sxs-lookup"><span data-stu-id="25bbb-103">List microsoftStoreForBusinessApps</span></span>

> <span data-ttu-id="25bbb-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="25bbb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25bbb-105">[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="25bbb-105">List properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="25bbb-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="25bbb-106">Prerequisites</span></span>
<span data-ttu-id="25bbb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25bbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25bbb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="25bbb-109">Permission type</span></span>|<span data-ttu-id="25bbb-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="25bbb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25bbb-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="25bbb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25bbb-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="25bbb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="25bbb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="25bbb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25bbb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25bbb-114">Not supported.</span></span>|
|<span data-ttu-id="25bbb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="25bbb-115">Application</span></span>|<span data-ttu-id="25bbb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25bbb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25bbb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="25bbb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="25bbb-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="25bbb-118">Request headers</span></span>
|<span data-ttu-id="25bbb-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="25bbb-119">Header</span></span>|<span data-ttu-id="25bbb-120">値</span><span class="sxs-lookup"><span data-stu-id="25bbb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25bbb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25bbb-121">Authorization</span></span>|<span data-ttu-id="25bbb-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="25bbb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25bbb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="25bbb-123">Accept</span></span>|<span data-ttu-id="25bbb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="25bbb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25bbb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="25bbb-125">Request body</span></span>
<span data-ttu-id="25bbb-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="25bbb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25bbb-127">応答</span><span class="sxs-lookup"><span data-stu-id="25bbb-127">Response</span></span>
<span data-ttu-id="25bbb-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="25bbb-128">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25bbb-129">例</span><span class="sxs-lookup"><span data-stu-id="25bbb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="25bbb-130">要求</span><span class="sxs-lookup"><span data-stu-id="25bbb-130">Request</span></span>
<span data-ttu-id="25bbb-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="25bbb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="25bbb-132">応答</span><span class="sxs-lookup"><span data-stu-id="25bbb-132">Response</span></span>
<span data-ttu-id="25bbb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="25bbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1070

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
      "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "productKey": "Product Key value",
      "licenseType": "online",
      "packageIdentityName": "Package Identity Name value"
    }
  ]
}
```



