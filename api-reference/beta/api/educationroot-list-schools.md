---
title: educationSchools をリストする
description: すべての学校オブジェクトのリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cf10d18188f09ee7c65195358e224f183ffd906e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515728"
---
# <a name="list-educationschools"></a><span data-ttu-id="141ec-103">educationSchools をリストする</span><span class="sxs-lookup"><span data-stu-id="141ec-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="141ec-104">すべての学校オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="141ec-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="141ec-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="141ec-105">Permissions</span></span>
<span data-ttu-id="141ec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="141ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="141ec-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="141ec-108">Permission type</span></span>      | <span data-ttu-id="141ec-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="141ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="141ec-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="141ec-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="141ec-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="141ec-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="141ec-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="141ec-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="141ec-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="141ec-113">Not supported.</span></span>  |
|<span data-ttu-id="141ec-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="141ec-114">Application</span></span> | <span data-ttu-id="141ec-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="141ec-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="141ec-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="141ec-116">HTTP request</span></span>
<span data-ttu-id="141ec-117"><!-- { "blockType": "ignored" } -->'' http GET/教育/学校</span><span class="sxs-lookup"><span data-stu-id="141ec-117"><!-- { "blockType": "ignored" } --> \`\`\`http GET /education/schools</span></span>
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
##### <a name="response"></a><span data-ttu-id="141ec-118">応答</span><span class="sxs-lookup"><span data-stu-id="141ec-118">Response</span></span>
<span data-ttu-id="141ec-119">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="141ec-119">The following is an example of the response.</span></span> 

><span data-ttu-id="141ec-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="141ec-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/educationroot-list-schools.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
