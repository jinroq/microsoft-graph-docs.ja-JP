---
title: Get managedEBook
description: managedEBook オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb3be61f932c2bd727af6808fb8b752f98c3438e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972278"
---
# <a name="get-managedebook"></a><span data-ttu-id="f83ae-103">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="f83ae-103">Get managedEBook</span></span>

> <span data-ttu-id="f83ae-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f83ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f83ae-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f83ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f83ae-106">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f83ae-106">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f83ae-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f83ae-107">Prerequisites</span></span>
<span data-ttu-id="f83ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f83ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f83ae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f83ae-110">Permission type</span></span>|<span data-ttu-id="f83ae-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f83ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f83ae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f83ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f83ae-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f83ae-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f83ae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f83ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f83ae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f83ae-115">Not supported.</span></span>|
|<span data-ttu-id="f83ae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f83ae-116">Application</span></span>|<span data-ttu-id="f83ae-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f83ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f83ae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f83ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f83ae-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f83ae-119">Optional query parameters</span></span>
<span data-ttu-id="f83ae-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f83ae-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f83ae-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f83ae-121">Request headers</span></span>
|<span data-ttu-id="f83ae-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f83ae-122">Header</span></span>|<span data-ttu-id="f83ae-123">値</span><span class="sxs-lookup"><span data-stu-id="f83ae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f83ae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f83ae-124">Authorization</span></span>|<span data-ttu-id="f83ae-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f83ae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f83ae-126">承諾</span><span class="sxs-lookup"><span data-stu-id="f83ae-126">Accept</span></span>|<span data-ttu-id="f83ae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f83ae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f83ae-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f83ae-128">Request body</span></span>
<span data-ttu-id="f83ae-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f83ae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f83ae-130">応答</span><span class="sxs-lookup"><span data-stu-id="f83ae-130">Response</span></span>
<span data-ttu-id="f83ae-131">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [managedEBook](../resources/intune-books-managedebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f83ae-131">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f83ae-132">例</span><span class="sxs-lookup"><span data-stu-id="f83ae-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f83ae-133">要求</span><span class="sxs-lookup"><span data-stu-id="f83ae-133">Request</span></span>
<span data-ttu-id="f83ae-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f83ae-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="f83ae-135">応答</span><span class="sxs-lookup"><span data-stu-id="f83ae-135">Response</span></span>
<span data-ttu-id="f83ae-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f83ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBook",
    "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
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
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
  }
}
```





