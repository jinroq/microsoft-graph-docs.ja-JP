---
title: メンバーを一覧表示する
description: クラスの教師と学生を取得します。 委任されたトークンを使用した場合、メンバーを参照できるのはクラスの他のメンバーのみになります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: db7013f2f98c9e36220a022a8ad5b3ea9f7c269f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370446"
---
# <a name="list-members"></a><span data-ttu-id="cc1b6-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cc1b6-104">List members</span></span>

<span data-ttu-id="cc1b6-105">クラスの教師と学生を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="cc1b6-106">委任されたトークンを使用した場合、メンバーを参照できるのはクラスの他のメンバーのみになります。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc1b6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc1b6-107">Permissions</span></span>
<span data-ttu-id="cc1b6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc1b6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc1b6-110">Permission type</span></span>      | <span data-ttu-id="cc1b6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc1b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc1b6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc1b6-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="cc1b6-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="cc1b6-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="cc1b6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc1b6-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cc1b6-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="cc1b6-115">Not supported</span></span>  |
|<span data-ttu-id="cc1b6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc1b6-116">Application</span></span> | <span data-ttu-id="cc1b6-117">Eduroster.readbasic、Eduroster.readbasic、およびすべての正の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cc1b6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc1b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc1b6-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cc1b6-119">Optional query parameters</span></span>
<span data-ttu-id="cc1b6-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc1b6-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc1b6-121">Request headers</span></span>
| <span data-ttu-id="cc1b6-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc1b6-122">Header</span></span>       | <span data-ttu-id="cc1b6-123">値</span><span class="sxs-lookup"><span data-stu-id="cc1b6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc1b6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc1b6-124">Authorization</span></span>  | <span data-ttu-id="cc1b6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc1b6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc1b6-127">Request body</span></span>
<span data-ttu-id="cc1b6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cc1b6-129">応答</span><span class="sxs-lookup"><span data-stu-id="cc1b6-129">Response</span></span>
<span data-ttu-id="cc1b6-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc1b6-131">例</span><span class="sxs-lookup"><span data-stu-id="cc1b6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc1b6-132">要求</span><span class="sxs-lookup"><span data-stu-id="cc1b6-132">Request</span></span>
<span data-ttu-id="cc1b6-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cc1b6-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cc1b6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc1b6-135">C#</span><span class="sxs-lookup"><span data-stu-id="cc1b6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc1b6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc1b6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc1b6-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="cc1b6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc1b6-138">Java</span><span class="sxs-lookup"><span data-stu-id="cc1b6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cc1b6-139">応答</span><span class="sxs-lookup"><span data-stu-id="cc1b6-139">Response</span></span>
<span data-ttu-id="cc1b6-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-140">The following is an example of the response.</span></span> 

><span data-ttu-id="cc1b6-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cc1b6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
