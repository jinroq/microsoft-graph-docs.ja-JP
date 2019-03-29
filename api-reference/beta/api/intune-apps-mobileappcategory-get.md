---
title: Get mobileAppCategory
description: mobileAppCategory オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17a39bb4f5845e98eb74db0ba45851017bf8ad71
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962170"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="a4c61-103">Get mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="a4c61-103">Get mobileAppCategory</span></span>

> <span data-ttu-id="a4c61-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4c61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4c61-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4c61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4c61-106">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a4c61-106">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4c61-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4c61-107">Prerequisites</span></span>
<span data-ttu-id="a4c61-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4c61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4c61-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4c61-110">Permission type</span></span>|<span data-ttu-id="a4c61-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4c61-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4c61-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4c61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4c61-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4c61-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a4c61-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4c61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4c61-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4c61-115">Not supported.</span></span>|
|<span data-ttu-id="a4c61-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4c61-116">Application</span></span>|<span data-ttu-id="a4c61-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4c61-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4c61-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4c61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4c61-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a4c61-119">Optional query parameters</span></span>
<span data-ttu-id="a4c61-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a4c61-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4c61-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4c61-121">Request headers</span></span>
|<span data-ttu-id="a4c61-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4c61-122">Header</span></span>|<span data-ttu-id="a4c61-123">値</span><span class="sxs-lookup"><span data-stu-id="a4c61-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4c61-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4c61-124">Authorization</span></span>|<span data-ttu-id="a4c61-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4c61-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4c61-126">承諾</span><span class="sxs-lookup"><span data-stu-id="a4c61-126">Accept</span></span>|<span data-ttu-id="a4c61-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a4c61-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4c61-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4c61-128">Request body</span></span>
<span data-ttu-id="a4c61-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a4c61-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4c61-130">応答</span><span class="sxs-lookup"><span data-stu-id="a4c61-130">Response</span></span>
<span data-ttu-id="a4c61-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4c61-131">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4c61-132">例</span><span class="sxs-lookup"><span data-stu-id="a4c61-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4c61-133">要求</span><span class="sxs-lookup"><span data-stu-id="a4c61-133">Request</span></span>
<span data-ttu-id="a4c61-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4c61-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="a4c61-135">応答</span><span class="sxs-lookup"><span data-stu-id="a4c61-135">Response</span></span>
<span data-ttu-id="a4c61-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a4c61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppCategory",
    "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




