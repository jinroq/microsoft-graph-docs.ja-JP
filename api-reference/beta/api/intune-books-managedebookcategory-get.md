---
title: ManagedEBookCategory の取得
description: ManagedEBookCategory オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 524297db637e5a7ce9f20888eb8cf8710038f0c5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328341"
---
# <a name="get-managedebookcategory"></a><span data-ttu-id="21ac4-103">ManagedEBookCategory の取得</span><span class="sxs-lookup"><span data-stu-id="21ac4-103">Get managedEBookCategory</span></span>

> <span data-ttu-id="21ac4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21ac4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21ac4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="21ac4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21ac4-106">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="21ac4-106">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21ac4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="21ac4-107">Prerequisites</span></span>
<span data-ttu-id="21ac4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21ac4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21ac4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="21ac4-110">Permission type</span></span>|<span data-ttu-id="21ac4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="21ac4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21ac4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="21ac4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21ac4-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21ac4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="21ac4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="21ac4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21ac4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21ac4-115">Not supported.</span></span>|
|<span data-ttu-id="21ac4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="21ac4-116">Application</span></span>|<span data-ttu-id="21ac4-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21ac4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21ac4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21ac4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21ac4-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="21ac4-119">Optional query parameters</span></span>
<span data-ttu-id="21ac4-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="21ac4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21ac4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21ac4-121">Request headers</span></span>
|<span data-ttu-id="21ac4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21ac4-122">Header</span></span>|<span data-ttu-id="21ac4-123">値</span><span class="sxs-lookup"><span data-stu-id="21ac4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21ac4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="21ac4-124">Authorization</span></span>|<span data-ttu-id="21ac4-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="21ac4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21ac4-126">承諾</span><span class="sxs-lookup"><span data-stu-id="21ac4-126">Accept</span></span>|<span data-ttu-id="21ac4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="21ac4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21ac4-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="21ac4-128">Request body</span></span>
<span data-ttu-id="21ac4-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="21ac4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21ac4-130">応答</span><span class="sxs-lookup"><span data-stu-id="21ac4-130">Response</span></span>
<span data-ttu-id="21ac4-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="21ac4-131">If successful, this method returns a `200 OK` response code and [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21ac4-132">例</span><span class="sxs-lookup"><span data-stu-id="21ac4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="21ac4-133">要求</span><span class="sxs-lookup"><span data-stu-id="21ac4-133">Request</span></span>
<span data-ttu-id="21ac4-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="21ac4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
```

### <a name="response"></a><span data-ttu-id="21ac4-135">応答</span><span class="sxs-lookup"><span data-stu-id="21ac4-135">Response</span></span>
<span data-ttu-id="21ac4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="21ac4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookCategory",
    "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```






