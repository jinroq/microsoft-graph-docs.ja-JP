---
title: mobileAppCategories のリスト
description: mobileAppCategory オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 7c18d2ee37b4012fdb19edfdc1efdbf01ce2200c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023867"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="433e0-103">mobileAppCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="433e0-103">List mobileAppCategories</span></span>

> <span data-ttu-id="433e0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="433e0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="433e0-105">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="433e0-105">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="433e0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="433e0-106">Prerequisites</span></span>
<span data-ttu-id="433e0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="433e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="433e0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="433e0-109">Permission type</span></span>|<span data-ttu-id="433e0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="433e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="433e0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="433e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="433e0-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="433e0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="433e0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="433e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="433e0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="433e0-114">Not supported.</span></span>|
|<span data-ttu-id="433e0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="433e0-115">Application</span></span>|<span data-ttu-id="433e0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="433e0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="433e0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="433e0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="433e0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="433e0-118">Request headers</span></span>
|<span data-ttu-id="433e0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="433e0-119">Header</span></span>|<span data-ttu-id="433e0-120">値</span><span class="sxs-lookup"><span data-stu-id="433e0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="433e0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="433e0-121">Authorization</span></span>|<span data-ttu-id="433e0-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="433e0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="433e0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="433e0-123">Accept</span></span>|<span data-ttu-id="433e0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="433e0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="433e0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="433e0-125">Request body</span></span>
<span data-ttu-id="433e0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="433e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="433e0-127">応答</span><span class="sxs-lookup"><span data-stu-id="433e0-127">Response</span></span>
<span data-ttu-id="433e0-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="433e0-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="433e0-129">例</span><span class="sxs-lookup"><span data-stu-id="433e0-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="433e0-130">要求</span><span class="sxs-lookup"><span data-stu-id="433e0-130">Request</span></span>
<span data-ttu-id="433e0-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="433e0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="433e0-132">応答</span><span class="sxs-lookup"><span data-stu-id="433e0-132">Response</span></span>
<span data-ttu-id="433e0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="433e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppCategory",
      "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```



