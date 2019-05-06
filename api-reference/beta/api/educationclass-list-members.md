---
title: メンバーを一覧表示する
description: クラスの教師と学生を取得します。 委任されたトークンを使用した場合、メンバーを参照できるのはクラスの他のメンバーのみになります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 6b563e144374eb026ab1c91698b49d9da75a5935
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587505"
---
# <a name="list-members"></a><span data-ttu-id="254aa-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="254aa-104">List members</span></span>

<span data-ttu-id="254aa-105">クラスの教師と学生を取得します。</span><span class="sxs-lookup"><span data-stu-id="254aa-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="254aa-106">委任されたトークンを使用した場合、メンバーを参照できるのはクラスの他のメンバーのみになります。</span><span class="sxs-lookup"><span data-stu-id="254aa-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="254aa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="254aa-107">Permissions</span></span>
<span data-ttu-id="254aa-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="254aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="254aa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="254aa-110">Permission type</span></span>      | <span data-ttu-id="254aa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="254aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="254aa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="254aa-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="254aa-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="254aa-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="254aa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="254aa-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="254aa-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="254aa-115">Not supported</span></span>  |
|<span data-ttu-id="254aa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="254aa-116">Application</span></span> | <span data-ttu-id="254aa-117">Eduroster.readbasic、Eduroster.readbasic、およびすべての正の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="254aa-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="254aa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="254aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="254aa-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="254aa-119">Optional query parameters</span></span>
<span data-ttu-id="254aa-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="254aa-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="254aa-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="254aa-121">Request headers</span></span>
| <span data-ttu-id="254aa-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="254aa-122">Header</span></span>       | <span data-ttu-id="254aa-123">値</span><span class="sxs-lookup"><span data-stu-id="254aa-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="254aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="254aa-124">Authorization</span></span>  | <span data-ttu-id="254aa-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="254aa-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="254aa-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="254aa-127">Request body</span></span>
<span data-ttu-id="254aa-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="254aa-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="254aa-129">応答</span><span class="sxs-lookup"><span data-stu-id="254aa-129">Response</span></span>
<span data-ttu-id="254aa-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="254aa-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="254aa-131">例</span><span class="sxs-lookup"><span data-stu-id="254aa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="254aa-132">要求</span><span class="sxs-lookup"><span data-stu-id="254aa-132">Request</span></span>
<span data-ttu-id="254aa-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="254aa-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
##### <a name="response"></a><span data-ttu-id="254aa-134">応答</span><span class="sxs-lookup"><span data-stu-id="254aa-134">Response</span></span>
<span data-ttu-id="254aa-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="254aa-135">The following is an example of the response.</span></span> 

><span data-ttu-id="254aa-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="254aa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="254aa-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="254aa-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="254aa-139">Visual</span><span class="sxs-lookup"><span data-stu-id="254aa-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="254aa-140">Java</span><span class="sxs-lookup"><span data-stu-id="254aa-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
