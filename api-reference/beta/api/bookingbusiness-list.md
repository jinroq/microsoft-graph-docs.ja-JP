---
title: BookingBusinesses のリスト
description: テナント用に作成された bookingbusiness オブジェクトのコレクションを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f1092d2d811591b5e5a05931e38264a8150d4d8c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415534"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="1e0bf-103">BookingBusinesses のリスト</span><span class="sxs-lookup"><span data-stu-id="1e0bf-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e0bf-104">テナント用に作成された[bookingbusiness](../resources/bookingbusiness.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="1e0bf-105">この操作では、コレクション内の各予約業務の**id**と**displayName**のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="1e0bf-106">パフォーマンスに関する考慮事項として、他のプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="1e0bf-107">[Get](bookingbusiness-get.md)操作でその**id**を指定することにより、予約ビジネスのその他のプロパティを取得できます。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="1e0bf-108">テナントのビジネス間で部分文字列の一致を実行するため`query`に、パラメーターに文字列を指定して、予約企業を照会することもできます。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="1e0bf-109">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="1e0bf-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e0bf-110">Permissions</span></span>
<span data-ttu-id="1e0bf-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e0bf-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e0bf-113">Permission type</span></span>      | <span data-ttu-id="1e0bf-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e0bf-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e0bf-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e0bf-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="1e0bf-116">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1e0bf-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e0bf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e0bf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-118">Not supported.</span></span>   |
|<span data-ttu-id="1e0bf-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e0bf-119">Application</span></span> | <span data-ttu-id="1e0bf-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1e0bf-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e0bf-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e0bf-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e0bf-122">Optional query parameters</span></span>
<span data-ttu-id="1e0bf-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1e0bf-124">このメソッドは、文字列`query`型 (string) の値を受け取るパラメーターもサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="1e0bf-125">このパラメーターは、指定した文字列に一致する企業に対して GET 結果を制限します。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="1e0bf-126">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="1e0bf-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e0bf-127">Request headers</span></span>
| <span data-ttu-id="1e0bf-128">名前</span><span class="sxs-lookup"><span data-stu-id="1e0bf-128">Name</span></span>      |<span data-ttu-id="1e0bf-129">説明</span><span class="sxs-lookup"><span data-stu-id="1e0bf-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e0bf-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e0bf-130">Authorization</span></span>  | <span data-ttu-id="1e0bf-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1e0bf-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e0bf-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e0bf-132">Request body</span></span>
<span data-ttu-id="1e0bf-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1e0bf-134">応答</span><span class="sxs-lookup"><span data-stu-id="1e0bf-134">Response</span></span>
<span data-ttu-id="1e0bf-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingbusiness](../resources/bookingbusiness.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e0bf-136">例</span><span class="sxs-lookup"><span data-stu-id="1e0bf-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="1e0bf-137">要求 1</span><span class="sxs-lookup"><span data-stu-id="1e0bf-137">Request 1</span></span>
<span data-ttu-id="1e0bf-138">次の例では、テナント内の予約企業を取得します。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-138">The following example gets the Bookings businesses in a tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e0bf-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1e0bf-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e0bf-140">C#</span><span class="sxs-lookup"><span data-stu-id="1e0bf-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e0bf-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e0bf-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e0bf-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="1e0bf-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="1e0bf-143">応答 1</span><span class="sxs-lookup"><span data-stu-id="1e0bf-143">Response 1</span></span>
<span data-ttu-id="1e0bf-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@M365B489948.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@M365B489948.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="1e0bf-145">要求 2</span><span class="sxs-lookup"><span data-stu-id="1e0bf-145">Request 2</span></span>
<span data-ttu-id="1e0bf-146">次の例は、 `query`パラメーターを使用して、テナント内の1つ以上の一致する予約企業を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-146">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e0bf-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1e0bf-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e0bf-148">C#</span><span class="sxs-lookup"><span data-stu-id="1e0bf-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/query-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e0bf-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e0bf-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/query-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e0bf-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="1e0bf-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/query-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="1e0bf-151">応答 2</span><span class="sxs-lookup"><span data-stu-id="1e0bf-151">Response 2</span></span>
<span data-ttu-id="1e0bf-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e0bf-152">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
