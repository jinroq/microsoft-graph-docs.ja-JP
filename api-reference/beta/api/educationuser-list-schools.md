---
title: 学校をリストする
description: ユーザーの学校のリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4486dce1155bf63eecf5ad5c4b1aa0f4fa20b4d7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259326"
---
# <a name="list-schools"></a><span data-ttu-id="956ae-103">学校をリストする</span><span class="sxs-lookup"><span data-stu-id="956ae-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="956ae-104">ユーザーの学校のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="956ae-104">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="956ae-105">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="956ae-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="956ae-106">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="956ae-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="956ae-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="956ae-107">Permissions</span></span>
<span data-ttu-id="956ae-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="956ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="956ae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="956ae-110">Permission type</span></span>      | <span data-ttu-id="956ae-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="956ae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="956ae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="956ae-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="956ae-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="956ae-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="956ae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="956ae-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="956ae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="956ae-115">Not supported.</span></span>  |
|<span data-ttu-id="956ae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="956ae-116">Application</span></span> | <span data-ttu-id="956ae-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956ae-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="956ae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="956ae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="956ae-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="956ae-119">Optional query parameters</span></span>
<span data-ttu-id="956ae-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="956ae-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="956ae-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="956ae-121">Request headers</span></span>
| <span data-ttu-id="956ae-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="956ae-122">Header</span></span>       | <span data-ttu-id="956ae-123">値</span><span class="sxs-lookup"><span data-stu-id="956ae-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="956ae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="956ae-124">Authorization</span></span>  | <span data-ttu-id="956ae-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="956ae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="956ae-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="956ae-127">Request body</span></span>
<span data-ttu-id="956ae-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="956ae-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="956ae-129">応答</span><span class="sxs-lookup"><span data-stu-id="956ae-129">Response</span></span>
<span data-ttu-id="956ae-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="956ae-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="956ae-131">例</span><span class="sxs-lookup"><span data-stu-id="956ae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="956ae-132">要求</span><span class="sxs-lookup"><span data-stu-id="956ae-132">Request</span></span>
<span data-ttu-id="956ae-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="956ae-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="956ae-134">応答</span><span class="sxs-lookup"><span data-stu-id="956ae-134">Response</span></span>
<span data-ttu-id="956ae-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="956ae-135">The following is an example of the response.</span></span> 

><span data-ttu-id="956ae-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="956ae-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="956ae-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="956ae-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="956ae-139">C#</span><span class="sxs-lookup"><span data-stu-id="956ae-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_schools-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="956ae-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="956ae-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_schools-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="956ae-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="956ae-141">Objective-C</span></span>](#tab/objective-c)
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
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
