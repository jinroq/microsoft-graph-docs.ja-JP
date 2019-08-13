---
title: 学校をリストする
description: ユーザーの学校のリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ab4cd6095ec489e012a60ab8dda17fa65062abe8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327088"
---
# <a name="list-schools"></a><span data-ttu-id="7c67c-103">学校をリストする</span><span class="sxs-lookup"><span data-stu-id="7c67c-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c67c-104">ユーザーの学校のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7c67c-104">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="7c67c-105">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="7c67c-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="7c67c-106">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="7c67c-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c67c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c67c-107">Permissions</span></span>
<span data-ttu-id="7c67c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c67c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c67c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c67c-110">Permission type</span></span>      | <span data-ttu-id="7c67c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c67c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c67c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c67c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="7c67c-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="7c67c-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="7c67c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c67c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7c67c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c67c-115">Not supported.</span></span>  |
|<span data-ttu-id="7c67c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c67c-116">Application</span></span> | <span data-ttu-id="7c67c-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c67c-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7c67c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c67c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7c67c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7c67c-119">Optional query parameters</span></span>
<span data-ttu-id="7c67c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7c67c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c67c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c67c-121">Request headers</span></span>
| <span data-ttu-id="7c67c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c67c-122">Header</span></span>       | <span data-ttu-id="7c67c-123">値</span><span class="sxs-lookup"><span data-stu-id="7c67c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c67c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c67c-124">Authorization</span></span>  | <span data-ttu-id="7c67c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c67c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c67c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c67c-127">Request body</span></span>
<span data-ttu-id="7c67c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7c67c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7c67c-129">応答</span><span class="sxs-lookup"><span data-stu-id="7c67c-129">Response</span></span>
<span data-ttu-id="7c67c-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7c67c-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7c67c-131">例</span><span class="sxs-lookup"><span data-stu-id="7c67c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c67c-132">要求</span><span class="sxs-lookup"><span data-stu-id="7c67c-132">Request</span></span>
<span data-ttu-id="7c67c-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c67c-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7c67c-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7c67c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7c67c-135">C#</span><span class="sxs-lookup"><span data-stu-id="7c67c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c67c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c67c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c67c-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="7c67c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7c67c-138">Java</span><span class="sxs-lookup"><span data-stu-id="7c67c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7c67c-139">応答</span><span class="sxs-lookup"><span data-stu-id="7c67c-139">Response</span></span>
<span data-ttu-id="7c67c-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c67c-140">The following is an example of the response.</span></span> 

><span data-ttu-id="7c67c-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7c67c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
