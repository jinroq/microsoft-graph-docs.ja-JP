---
title: ユーザーを一覧表示する
description: ユーザー オブジェクトの一覧を取得します。 これらのユーザーオブジェクトには、教育機関に固有のプロパティが含まれます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 10ec2434232b963e3e88a6e52134e4550edff4b5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616195"
---
# <a name="list-users"></a><span data-ttu-id="3b7c2-104">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3b7c2-104">List users</span></span>

<span data-ttu-id="3b7c2-105">ユーザー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="3b7c2-106">これらのユーザーオブジェクトには、教育機関に固有のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b7c2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b7c2-107">Permissions</span></span>
<span data-ttu-id="3b7c2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b7c2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b7c2-110">Permission type</span></span>      | <span data-ttu-id="3b7c2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b7c2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b7c2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b7c2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3b7c2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-113">Not supported.</span></span>  |
|<span data-ttu-id="3b7c2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b7c2-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3b7c2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-115">Not supported.</span></span>  |
|<span data-ttu-id="3b7c2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b7c2-116">Application</span></span> | <span data-ttu-id="3b7c2-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b7c2-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3b7c2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b7c2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b7c2-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3b7c2-119">Optional query parameters</span></span>
<span data-ttu-id="3b7c2-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b7c2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b7c2-121">Request headers</span></span>
| <span data-ttu-id="3b7c2-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b7c2-122">Header</span></span>       | <span data-ttu-id="3b7c2-123">値</span><span class="sxs-lookup"><span data-stu-id="3b7c2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b7c2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b7c2-124">Authorization</span></span>  | <span data-ttu-id="3b7c2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b7c2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b7c2-127">Request body</span></span>
<span data-ttu-id="3b7c2-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3b7c2-129">応答</span><span class="sxs-lookup"><span data-stu-id="3b7c2-129">Response</span></span>
<span data-ttu-id="3b7c2-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b7c2-131">例</span><span class="sxs-lookup"><span data-stu-id="3b7c2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b7c2-132">要求</span><span class="sxs-lookup"><span data-stu-id="3b7c2-132">Request</span></span>
<span data-ttu-id="3b7c2-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users
```
##### <a name="response"></a><span data-ttu-id="3b7c2-134">応答</span><span class="sxs-lookup"><span data-stu-id="3b7c2-134">Response</span></span>
<span data-ttu-id="3b7c2-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="3b7c2-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3b7c2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": null,
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3b7c2-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="3b7c2-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3b7c2-139">Visual</span><span class="sxs-lookup"><span data-stu-id="3b7c2-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b7c2-140">Java</span><span class="sxs-lookup"><span data-stu-id="3b7c2-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
