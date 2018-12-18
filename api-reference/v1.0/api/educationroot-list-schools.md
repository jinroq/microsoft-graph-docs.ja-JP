---
title: educationSchools をリストする
description: すべての学校オブジェクトのリストを取得します。
author: mmast-msft
ms.openlocfilehash: 361c0ae0f15244b78fcbd13bc7c190c0e53bf079
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305874"
---
# <a name="list-educationschools"></a><span data-ttu-id="229d5-103">educationSchools をリストする</span><span class="sxs-lookup"><span data-stu-id="229d5-103">List educationSchools</span></span>

<span data-ttu-id="229d5-104">すべての学校オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="229d5-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="229d5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="229d5-105">Permissions</span></span>
<span data-ttu-id="229d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="229d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="229d5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="229d5-108">Permission type</span></span>      | <span data-ttu-id="229d5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="229d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="229d5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="229d5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="229d5-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="229d5-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="229d5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="229d5-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="229d5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="229d5-113">Not supported.</span></span>  |
|<span data-ttu-id="229d5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="229d5-114">Application</span></span> | <span data-ttu-id="229d5-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="229d5-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="229d5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="229d5-116">HTTP request</span></span>
<span data-ttu-id="229d5-117"><!-- { "blockType": "ignored" } -->'' http GET/教育/学校</span><span class="sxs-lookup"><span data-stu-id="229d5-117"><!-- { "blockType": "ignored" } --> \`\`\`http GET /education/schools</span></span>
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
GET https://graph.microsoft.com/v1.0/education/schools
```
##### <a name="response"></a><span data-ttu-id="229d5-118">応答</span><span class="sxs-lookup"><span data-stu-id="229d5-118">Response</span></span>
<span data-ttu-id="229d5-119">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="229d5-119">The following is an example of the response.</span></span> 

><span data-ttu-id="229d5-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="229d5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
