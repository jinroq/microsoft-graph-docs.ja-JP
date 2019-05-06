---
title: educationUsers をリストする
description: 学校のユーザーのリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2432c78c966da2402f2fd753c02a9d0b900ff656
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587909"
---
# <a name="list-educationusers"></a><span data-ttu-id="0c56e-103">educationUsers をリストする</span><span class="sxs-lookup"><span data-stu-id="0c56e-103">List educationUsers</span></span>

<span data-ttu-id="0c56e-104">学校のユーザーのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="0c56e-104">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c56e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c56e-105">Permissions</span></span>
<span data-ttu-id="0c56e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c56e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c56e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c56e-108">Permission type</span></span>      | <span data-ttu-id="0c56e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c56e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c56e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c56e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c56e-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c56e-111">Not supported.</span></span>  |
|<span data-ttu-id="0c56e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c56e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c56e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c56e-113">Not supported.</span></span>  |
|<span data-ttu-id="0c56e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c56e-114">Application</span></span> | <span data-ttu-id="0c56e-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c56e-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c56e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c56e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0c56e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c56e-117">Optional query parameters</span></span>
<span data-ttu-id="0c56e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0c56e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c56e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c56e-119">Request headers</span></span>
| <span data-ttu-id="0c56e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c56e-120">Header</span></span>       | <span data-ttu-id="0c56e-121">値</span><span class="sxs-lookup"><span data-stu-id="0c56e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c56e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c56e-122">Authorization</span></span>  | <span data-ttu-id="0c56e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0c56e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c56e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c56e-125">Request body</span></span>
<span data-ttu-id="0c56e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0c56e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0c56e-127">応答</span><span class="sxs-lookup"><span data-stu-id="0c56e-127">Response</span></span>
<span data-ttu-id="0c56e-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0c56e-128">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c56e-129">例</span><span class="sxs-lookup"><span data-stu-id="0c56e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c56e-130">要求</span><span class="sxs-lookup"><span data-stu-id="0c56e-130">Request</span></span>
<span data-ttu-id="0c56e-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c56e-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
##### <a name="response"></a><span data-ttu-id="0c56e-132">応答</span><span class="sxs-lookup"><span data-stu-id="0c56e-132">Response</span></span>
<span data-ttu-id="0c56e-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c56e-133">The following is an example of the response.</span></span> 

><span data-ttu-id="0c56e-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0c56e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "middleName": " ",
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0c56e-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="0c56e-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0c56e-137">Visual</span><span class="sxs-lookup"><span data-stu-id="0c56e-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c56e-138">Java</span><span class="sxs-lookup"><span data-stu-id="0c56e-138">Javascript</span></span>](#tab/javascript)
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
    "Error: /api-reference/v1.0/api/educationschool-list-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationschool-list-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
