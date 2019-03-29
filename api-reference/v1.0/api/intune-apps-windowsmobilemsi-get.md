---
title: Get windowsMobileMSI
description: windowsMobileMSI オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbe9088261e76cd687ed6ae2dd7cd576f0b63173
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975330"
---
# <a name="get-windowsmobilemsi"></a><span data-ttu-id="ffb80-103">Get windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="ffb80-103">Get windowsMobileMSI</span></span>

> <span data-ttu-id="ffb80-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffb80-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffb80-105">[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ffb80-105">Read properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffb80-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ffb80-106">Prerequisites</span></span>
<span data-ttu-id="ffb80-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffb80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffb80-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffb80-109">Permission type</span></span>|<span data-ttu-id="ffb80-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffb80-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffb80-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffb80-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ffb80-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffb80-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ffb80-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ffb80-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffb80-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffb80-114">Not supported.</span></span>|
|<span data-ttu-id="ffb80-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffb80-115">Application</span></span>|<span data-ttu-id="ffb80-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffb80-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffb80-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffb80-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffb80-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ffb80-118">Optional query parameters</span></span>
<span data-ttu-id="ffb80-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ffb80-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffb80-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffb80-120">Request headers</span></span>
|<span data-ttu-id="ffb80-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffb80-121">Header</span></span>|<span data-ttu-id="ffb80-122">値</span><span class="sxs-lookup"><span data-stu-id="ffb80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffb80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffb80-123">Authorization</span></span>|<span data-ttu-id="ffb80-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffb80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffb80-125">承諾</span><span class="sxs-lookup"><span data-stu-id="ffb80-125">Accept</span></span>|<span data-ttu-id="ffb80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffb80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb80-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ffb80-127">Request body</span></span>
<span data-ttu-id="ffb80-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ffb80-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffb80-129">応答</span><span class="sxs-lookup"><span data-stu-id="ffb80-129">Response</span></span>
<span data-ttu-id="ffb80-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ffb80-130">If successful, this method returns a `200 OK` response code and [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb80-131">例</span><span class="sxs-lookup"><span data-stu-id="ffb80-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffb80-132">要求</span><span class="sxs-lookup"><span data-stu-id="ffb80-132">Request</span></span>
<span data-ttu-id="ffb80-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ffb80-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ffb80-134">応答</span><span class="sxs-lookup"><span data-stu-id="ffb80-134">Response</span></span>
<span data-ttu-id="ffb80-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ffb80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1098

{
  "value": {
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
}
```



