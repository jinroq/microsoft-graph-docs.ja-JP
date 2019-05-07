---
title: BookingBusinesses のリスト
description: テナント用に作成された bookingbusiness オブジェクトのコレクションを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6a8b10582ab6455184a60272afb9b3bbe97daf4a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636164"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="e6f0c-103">BookingBusinesses のリスト</span><span class="sxs-lookup"><span data-stu-id="e6f0c-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6f0c-104">テナント用に作成された[bookingbusiness](../resources/bookingbusiness.md)オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="e6f0c-105">この操作では、コレクション内の各予約業務の**id**と**displayName**のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="e6f0c-106">パフォーマンスに関する考慮事項として、他のプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="e6f0c-107">[Get](bookingbusiness-get.md)操作でその**id**を指定することにより、予約ビジネスのその他のプロパティを取得できます。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="e6f0c-108">テナントのビジネス間で部分文字列の一致を実行するため`query`に、パラメーターに文字列を指定して、予約企業を照会することもできます。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="e6f0c-109">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="e6f0c-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e6f0c-110">Permissions</span></span>
<span data-ttu-id="e6f0c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6f0c-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6f0c-113">Permission type</span></span>      | <span data-ttu-id="e6f0c-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6f0c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6f0c-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6f0c-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6f0c-116">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e6f0c-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6f0c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6f0c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-118">Not supported.</span></span>   |
|<span data-ttu-id="e6f0c-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6f0c-119">Application</span></span> | <span data-ttu-id="e6f0c-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e6f0c-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6f0c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6f0c-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e6f0c-122">Optional query parameters</span></span>
<span data-ttu-id="e6f0c-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e6f0c-124">このメソッドは、文字列`query`型 (string) の値を受け取るパラメーターもサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="e6f0c-125">このパラメーターは、指定した文字列に一致する企業に対して GET 結果を制限します。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="e6f0c-126">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="e6f0c-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6f0c-127">Request headers</span></span>
| <span data-ttu-id="e6f0c-128">名前</span><span class="sxs-lookup"><span data-stu-id="e6f0c-128">Name</span></span>      |<span data-ttu-id="e6f0c-129">説明</span><span class="sxs-lookup"><span data-stu-id="e6f0c-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6f0c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6f0c-130">Authorization</span></span>  | <span data-ttu-id="e6f0c-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e6f0c-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6f0c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6f0c-132">Request body</span></span>
<span data-ttu-id="e6f0c-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e6f0c-134">応答</span><span class="sxs-lookup"><span data-stu-id="e6f0c-134">Response</span></span>
<span data-ttu-id="e6f0c-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingbusiness](../resources/bookingbusiness.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6f0c-136">例</span><span class="sxs-lookup"><span data-stu-id="e6f0c-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e6f0c-137">要求 1</span><span class="sxs-lookup"><span data-stu-id="e6f0c-137">Request 1</span></span>
<span data-ttu-id="e6f0c-138">次の例では、テナント内の予約企業を取得します。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="e6f0c-139">応答 1</span><span class="sxs-lookup"><span data-stu-id="e6f0c-139">Response 1</span></span>
<span data-ttu-id="e6f0c-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-140">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6f0c-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e6f0c-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6f0c-142">Visual</span><span class="sxs-lookup"><span data-stu-id="e6f0c-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingbusinesses-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6f0c-143">Java</span><span class="sxs-lookup"><span data-stu-id="e6f0c-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingbusinesses-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a><span data-ttu-id="e6f0c-144">要求 2</span><span class="sxs-lookup"><span data-stu-id="e6f0c-144">Request 2</span></span>
<span data-ttu-id="e6f0c-145">次の例は、 `query`パラメーターを使用して、テナント内の1つ以上の一致する予約企業を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-145">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="e6f0c-146">応答 2</span><span class="sxs-lookup"><span data-stu-id="e6f0c-146">Response 2</span></span>
<span data-ttu-id="e6f0c-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e6f0c-147">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6f0c-148">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e6f0c-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6f0c-149">Visual</span><span class="sxs-lookup"><span data-stu-id="e6f0c-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/query_bookingbusinesses-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6f0c-150">Java</span><span class="sxs-lookup"><span data-stu-id="e6f0c-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/query_bookingbusinesses-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
