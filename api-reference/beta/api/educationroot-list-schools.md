---
title: educationSchools をリストする
description: すべての学校オブジェクトのリストを取得します。
author: mmast-msft
ms.openlocfilehash: 98b3dcd1421ab42d88dbbf831b69ba9591337052
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363649"
---
# <a name="list-educationschools"></a><span data-ttu-id="358db-103">educationSchools をリストする</span><span class="sxs-lookup"><span data-stu-id="358db-103">List educationSchools</span></span>

> <span data-ttu-id="358db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="358db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="358db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="358db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="358db-106">すべての学校オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="358db-106">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="358db-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="358db-107">Permissions</span></span>
<span data-ttu-id="358db-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="358db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="358db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="358db-110">Permission type</span></span>      | <span data-ttu-id="358db-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="358db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="358db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="358db-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="358db-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="358db-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="358db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="358db-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="358db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="358db-115">Not supported.</span></span>  |
|<span data-ttu-id="358db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="358db-116">Application</span></span> | <span data-ttu-id="358db-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="358db-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="358db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="358db-118">HTTP request</span></span>
<span data-ttu-id="358db-119"><!-- { "blockType": "ignored" } -->'' http GET/教育/学校</span><span class="sxs-lookup"><span data-stu-id="358db-119"><!-- { "blockType": "ignored" } --> \`\`\`http GET /education/schools</span></span>
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
##### <a name="response"></a><span data-ttu-id="358db-120">応答</span><span class="sxs-lookup"><span data-stu-id="358db-120">Response</span></span>
<span data-ttu-id="358db-121">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="358db-121">The following is an example of the response.</span></span> 

><span data-ttu-id="358db-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="358db-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
