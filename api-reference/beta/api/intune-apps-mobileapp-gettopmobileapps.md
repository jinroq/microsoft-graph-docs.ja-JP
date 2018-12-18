---
title: getTopMobileApps 関数
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 03157e744358f4d76e781d33ae056104cf0a1130
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322730"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="b1afd-103">getTopMobileApps 関数</span><span class="sxs-lookup"><span data-stu-id="b1afd-103">getTopMobileApps function</span></span>

> <span data-ttu-id="b1afd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1afd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1afd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1afd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1afd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b1afd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1afd-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b1afd-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1afd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b1afd-108">Prerequisites</span></span>
<span data-ttu-id="b1afd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1afd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1afd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1afd-111">Permission type</span></span>|<span data-ttu-id="b1afd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1afd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1afd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1afd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1afd-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1afd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b1afd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1afd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1afd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1afd-116">Not supported.</span></span>|
|<span data-ttu-id="b1afd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1afd-117">Application</span></span>|<span data-ttu-id="b1afd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1afd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1afd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1afd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b1afd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1afd-120">Request headers</span></span>
|<span data-ttu-id="b1afd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1afd-121">Header</span></span>|<span data-ttu-id="b1afd-122">値</span><span class="sxs-lookup"><span data-stu-id="b1afd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1afd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1afd-123">Authorization</span></span>|<span data-ttu-id="b1afd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b1afd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1afd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1afd-125">Accept</span></span>|<span data-ttu-id="b1afd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1afd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1afd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1afd-127">Request body</span></span>
<span data-ttu-id="b1afd-128">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1afd-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b1afd-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="b1afd-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b1afd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1afd-130">Property</span></span>|<span data-ttu-id="b1afd-131">種類</span><span class="sxs-lookup"><span data-stu-id="b1afd-131">Type</span></span>|<span data-ttu-id="b1afd-132">説明</span><span class="sxs-lookup"><span data-stu-id="b1afd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1afd-133">status</span><span class="sxs-lookup"><span data-stu-id="b1afd-133">status</span></span>|<span data-ttu-id="b1afd-134">String</span><span class="sxs-lookup"><span data-stu-id="b1afd-134">String</span></span>|<span data-ttu-id="b1afd-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b1afd-135">Not yet documented</span></span>|
|<span data-ttu-id="b1afd-136">count</span><span class="sxs-lookup"><span data-stu-id="b1afd-136">count</span></span>|<span data-ttu-id="b1afd-137">Int64</span><span class="sxs-lookup"><span data-stu-id="b1afd-137">Int64</span></span>|<span data-ttu-id="b1afd-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b1afd-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1afd-139">応答</span><span class="sxs-lookup"><span data-stu-id="b1afd-139">Response</span></span>
<span data-ttu-id="b1afd-140">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に[mobileApp](../resources/intune-apps-mobileapp.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b1afd-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1afd-141">例</span><span class="sxs-lookup"><span data-stu-id="b1afd-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1afd-142">要求</span><span class="sxs-lookup"><span data-stu-id="b1afd-142">Request</span></span>
<span data-ttu-id="b1afd-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1afd-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="b1afd-144">応答</span><span class="sxs-lookup"><span data-stu-id="b1afd-144">Response</span></span>
<span data-ttu-id="b1afd-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1afd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 881

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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
      "publishingState": "processing"
    }
  ]
}
```





