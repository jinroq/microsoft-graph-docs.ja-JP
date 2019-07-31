---
title: リスト trendingAround
description: ユーザーの周囲でのアイテムのリストを返す、計算された洞察。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dc7b6176fe4fceeeeea78d63c6b7140568ff6875
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996190"
---
# <a name="list-trendingaround"></a><span data-ttu-id="12108-103">リスト trendingAround</span><span class="sxs-lookup"><span data-stu-id="12108-103">List trendingAround</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12108-104">ユーザーの周囲でのアイテムのリストを返す、計算された洞察。</span><span class="sxs-lookup"><span data-stu-id="12108-104">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="12108-105">**注:** この API は非推奨になり、[トレンド api](../resources/insights-trending.md)に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="12108-105">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="12108-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12108-106">Permissions</span></span>
<span data-ttu-id="12108-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12108-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12108-109">Permission type</span></span>      | <span data-ttu-id="12108-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="12108-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12108-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12108-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12108-112">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="12108-112">Sites.Read.All</span></span>    |
|<span data-ttu-id="12108-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12108-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12108-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12108-114">Not supported.</span></span>    |
|<span data-ttu-id="12108-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12108-115">Application</span></span> | <span data-ttu-id="12108-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="12108-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12108-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12108-117">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12108-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="12108-118">Optional query parameters</span></span>
<span data-ttu-id="12108-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="12108-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12108-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12108-120">Request headers</span></span>
| <span data-ttu-id="12108-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12108-121">Header</span></span>         | <span data-ttu-id="12108-122">値</span><span class="sxs-lookup"><span data-stu-id="12108-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="12108-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12108-123">Authorization</span></span>  | <span data-ttu-id="12108-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="12108-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12108-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12108-126">Content-Type</span></span>   | <span data-ttu-id="12108-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12108-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="12108-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="12108-128">Request body</span></span>
<span data-ttu-id="12108-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="12108-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12108-130">応答</span><span class="sxs-lookup"><span data-stu-id="12108-130">Response</span></span>

<span data-ttu-id="12108-131">成功した場合、このメソッドは、応答本文で 200 OK 応答コードと、[ハードアイテム](../resources/driveitem.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="12108-131">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12108-132">例</span><span class="sxs-lookup"><span data-stu-id="12108-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12108-133">要求</span><span class="sxs-lookup"><span data-stu-id="12108-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="12108-134">応答</span><span class="sxs-lookup"><span data-stu-id="12108-134">Response</span></span>
<span data-ttu-id="12108-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12108-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 226

{
  "id": "id-value",
  "name": "name-value",
  "DateTimeCreated": "DateTimeCreated-value",
  "DateTimeLastModified": "DateTimeLastModified-value",
  "webUrl": "webUrl-value",
}
```
