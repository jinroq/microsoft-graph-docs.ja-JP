---
title: 顧客を一覧表示する
description: BookingCustomer オブジェクトのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: cbe0d907e6d955c2d5df20bcfabd0f8ddcd68127
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318351"
---
# <a name="list-customers"></a><span data-ttu-id="6dcbe-103">顧客を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6dcbe-103">List customers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dcbe-104">[Bookingcustomer](../resources/bookingcustomer.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-104">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6dcbe-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6dcbe-105">Permissions</span></span>
<span data-ttu-id="6dcbe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dcbe-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6dcbe-108">Permission type</span></span>      | <span data-ttu-id="6dcbe-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6dcbe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dcbe-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6dcbe-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6dcbe-111">予約します。 all、BookingsAppointment すべての予約。すべての予約が可能です。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6dcbe-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6dcbe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dcbe-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-113">Not supported.</span></span>   |
|<span data-ttu-id="6dcbe-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6dcbe-114">Application</span></span> | <span data-ttu-id="6dcbe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6dcbe-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6dcbe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6dcbe-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6dcbe-117">Optional query parameters</span></span>
<span data-ttu-id="6dcbe-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dcbe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dcbe-119">Request headers</span></span>
| <span data-ttu-id="6dcbe-120">名前</span><span class="sxs-lookup"><span data-stu-id="6dcbe-120">Name</span></span>      |<span data-ttu-id="6dcbe-121">説明</span><span class="sxs-lookup"><span data-stu-id="6dcbe-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6dcbe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dcbe-122">Authorization</span></span>  | <span data-ttu-id="6dcbe-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6dcbe-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dcbe-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="6dcbe-124">Request body</span></span>
<span data-ttu-id="6dcbe-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6dcbe-126">応答</span><span class="sxs-lookup"><span data-stu-id="6dcbe-126">Response</span></span>
<span data-ttu-id="6dcbe-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[bookingcustomer](../resources/bookingcustomer.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-127">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6dcbe-128">例</span><span class="sxs-lookup"><span data-stu-id="6dcbe-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dcbe-129">要求</span><span class="sxs-lookup"><span data-stu-id="6dcbe-129">Request</span></span>
<span data-ttu-id="6dcbe-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6dcbe-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6dcbe-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dcbe-132">C#</span><span class="sxs-lookup"><span data-stu-id="6dcbe-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-customers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dcbe-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dcbe-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-customers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dcbe-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="6dcbe-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-customers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6dcbe-135">Java</span><span class="sxs-lookup"><span data-stu-id="6dcbe-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-customers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6dcbe-136">応答</span><span class="sxs-lookup"><span data-stu-id="6dcbe-136">Response</span></span>
<span data-ttu-id="6dcbe-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-137">The following is an example of the response.</span></span> <span data-ttu-id="6dcbe-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6dcbe-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6dcbe-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers",
    "value": [
        {
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com"
        },
        {
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
