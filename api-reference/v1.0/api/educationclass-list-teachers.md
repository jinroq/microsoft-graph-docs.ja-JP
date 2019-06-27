---
title: 教師をリストする
description: クラスの教師のリストを取得します。 教師のリストを取得するには、委任されたトークンがクラスのメンバーである必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 42ea0e0b4c65fdccc39a7e5ebdfe2186a9ec5183
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273011"
---
# <a name="list-teachers"></a><span data-ttu-id="fc5e4-104">教師をリストする</span><span class="sxs-lookup"><span data-stu-id="fc5e4-104">List teachers</span></span>

<span data-ttu-id="fc5e4-105">クラスの教師のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-105">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="fc5e4-106">教師のリストを取得するには、委任されたトークンがクラスのメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-106">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc5e4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fc5e4-107">Permissions</span></span>
<span data-ttu-id="fc5e4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc5e4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fc5e4-110">Permission type</span></span>      | <span data-ttu-id="fc5e4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fc5e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc5e4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fc5e4-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="fc5e4-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="fc5e4-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="fc5e4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fc5e4-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="fc5e4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-115">Not supported.</span></span>  |
|<span data-ttu-id="fc5e4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fc5e4-116">Application</span></span> | <span data-ttu-id="fc5e4-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc5e4-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fc5e4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fc5e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc5e4-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fc5e4-119">Optional query parameters</span></span>
<span data-ttu-id="fc5e4-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc5e4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc5e4-121">Request headers</span></span>
| <span data-ttu-id="fc5e4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc5e4-122">Header</span></span>       | <span data-ttu-id="fc5e4-123">値</span><span class="sxs-lookup"><span data-stu-id="fc5e4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc5e4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc5e4-124">Authorization</span></span>  | <span data-ttu-id="fc5e4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc5e4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fc5e4-127">Request body</span></span>
<span data-ttu-id="fc5e4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fc5e4-129">応答</span><span class="sxs-lookup"><span data-stu-id="fc5e4-129">Response</span></span>
<span data-ttu-id="fc5e4-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc5e4-131">例</span><span class="sxs-lookup"><span data-stu-id="fc5e4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc5e4-132">要求</span><span class="sxs-lookup"><span data-stu-id="fc5e4-132">Request</span></span>
<span data-ttu-id="fc5e4-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers
```
##### <a name="response"></a><span data-ttu-id="fc5e4-134">応答</span><span class="sxs-lookup"><span data-stu-id="fc5e4-134">Response</span></span>
<span data-ttu-id="fc5e4-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-135">The following is an example of the response.</span></span> 

><span data-ttu-id="fc5e4-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fc5e4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc5e4-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="fc5e4-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fc5e4-139">C#</span><span class="sxs-lookup"><span data-stu-id="fc5e4-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_teachers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc5e4-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc5e4-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_teachers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fc5e4-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="fc5e4-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_teachers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-list-teachers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationclass-list-teachers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-list-teachers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
