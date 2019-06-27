---
title: educationSchools をリストする
description: すべての学校オブジェクトのリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f1736f0b0369a0ffa55832a47b8fb7c022226638
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259697"
---
# <a name="list-educationschools"></a><span data-ttu-id="8d99d-103">educationSchools をリストする</span><span class="sxs-lookup"><span data-stu-id="8d99d-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d99d-104">すべての学校オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="8d99d-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d99d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d99d-105">Permissions</span></span>
<span data-ttu-id="8d99d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d99d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d99d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d99d-108">Permission type</span></span>      | <span data-ttu-id="8d99d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d99d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d99d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d99d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8d99d-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8d99d-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="8d99d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d99d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8d99d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d99d-113">Not supported.</span></span>  |
|<span data-ttu-id="8d99d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d99d-114">Application</span></span> | <span data-ttu-id="8d99d-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d99d-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8d99d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d99d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8d99d-117">\`\`\`http GET /education/schools</span><span class="sxs-lookup"><span data-stu-id="8d99d-117">\`\`\`http GET /education/schools</span></span>
```
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.

## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |

## Request body
Do not supply a request body for this method.
## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.
## Example
##### Request
The following is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools
```
##### <a name="response"></a><span data-ttu-id="8d99d-118">応答</span><span class="sxs-lookup"><span data-stu-id="8d99d-118">Response</span></span>
<span data-ttu-id="8d99d-119">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d99d-119">The following is an example of the response.</span></span> 

><span data-ttu-id="8d99d-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8d99d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d99d-122">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8d99d-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8d99d-123">C#</span><span class="sxs-lookup"><span data-stu-id="8d99d-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_schools-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d99d-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d99d-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_schools-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8d99d-125">目的-C</span><span class="sxs-lookup"><span data-stu-id="8d99d-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_schools-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationroot-list-schools.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationroot-list-schools.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationroot-list-schools.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
