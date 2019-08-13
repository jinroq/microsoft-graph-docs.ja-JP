---
title: ユーザーを一覧表示する
description: ユーザー オブジェクトの一覧を取得します。 これらのユーザーオブジェクトには、教育機関に固有のプロパティが含まれます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1cd20e9b628339d0004e29961649288b0d7aa2f8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323972"
---
# <a name="list-users"></a><span data-ttu-id="e7880-104">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e7880-104">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7880-105">ユーザー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7880-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="e7880-106">これらのユーザーオブジェクトには、教育機関に固有のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e7880-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7880-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7880-107">Permissions</span></span>
<span data-ttu-id="e7880-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7880-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7880-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7880-110">Permission type</span></span>      | <span data-ttu-id="e7880-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7880-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7880-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7880-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e7880-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7880-113">Not supported.</span></span>  |
|<span data-ttu-id="e7880-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7880-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e7880-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7880-115">Not supported.</span></span>  |
|<span data-ttu-id="e7880-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7880-116">Application</span></span> | <span data-ttu-id="e7880-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7880-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e7880-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7880-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7880-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7880-119">Optional query parameters</span></span>
<span data-ttu-id="e7880-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e7880-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7880-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7880-121">Request headers</span></span>
| <span data-ttu-id="e7880-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7880-122">Header</span></span>       | <span data-ttu-id="e7880-123">値</span><span class="sxs-lookup"><span data-stu-id="e7880-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7880-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7880-124">Authorization</span></span>  | <span data-ttu-id="e7880-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7880-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7880-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7880-127">Request body</span></span>
<span data-ttu-id="e7880-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7880-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e7880-129">応答</span><span class="sxs-lookup"><span data-stu-id="e7880-129">Response</span></span>
<span data-ttu-id="e7880-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e7880-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7880-131">例</span><span class="sxs-lookup"><span data-stu-id="e7880-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7880-132">要求</span><span class="sxs-lookup"><span data-stu-id="e7880-132">Request</span></span>
<span data-ttu-id="e7880-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7880-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e7880-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e7880-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationroot_get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7880-135">C#</span><span class="sxs-lookup"><span data-stu-id="e7880-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationroot-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7880-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7880-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationroot-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7880-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="e7880-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationroot-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7880-138">Java</span><span class="sxs-lookup"><span data-stu-id="e7880-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationroot-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7880-139">応答</span><span class="sxs-lookup"><span data-stu-id="e7880-139">Response</span></span>
<span data-ttu-id="e7880-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7880-140">The following is an example of the response.</span></span> 

><span data-ttu-id="e7880-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e7880-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
