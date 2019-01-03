---
title: 学校をリストする
description: ユーザーの学校のリストを取得します。
author: mmast-msft
ms.openlocfilehash: 6197096da6638f892c8a3819918d8f2bb6690afa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321988"
---
# <a name="list-schools"></a><span data-ttu-id="2d279-103">学校をリストする</span><span class="sxs-lookup"><span data-stu-id="2d279-103">List schools</span></span>

<span data-ttu-id="2d279-104">ユーザーの学校のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2d279-104">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="2d279-105">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="2d279-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="2d279-106">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="2d279-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d279-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2d279-107">Permissions</span></span>
<span data-ttu-id="2d279-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d279-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d279-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d279-110">Permission type</span></span>      | <span data-ttu-id="2d279-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d279-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d279-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d279-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2d279-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2d279-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2d279-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d279-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2d279-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d279-115">Not supported.</span></span>  |
|<span data-ttu-id="2d279-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d279-116">Application</span></span> | <span data-ttu-id="2d279-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d279-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2d279-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d279-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d279-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2d279-119">Optional query parameters</span></span>
<span data-ttu-id="2d279-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2d279-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d279-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d279-121">Request headers</span></span>
| <span data-ttu-id="2d279-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d279-122">Header</span></span>       | <span data-ttu-id="2d279-123">値</span><span class="sxs-lookup"><span data-stu-id="2d279-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d279-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d279-124">Authorization</span></span>  | <span data-ttu-id="2d279-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2d279-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d279-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d279-127">Request body</span></span>
<span data-ttu-id="2d279-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2d279-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2d279-129">応答</span><span class="sxs-lookup"><span data-stu-id="2d279-129">Response</span></span>
<span data-ttu-id="2d279-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2d279-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d279-131">例</span><span class="sxs-lookup"><span data-stu-id="2d279-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d279-132">要求</span><span class="sxs-lookup"><span data-stu-id="2d279-132">Request</span></span>
<span data-ttu-id="2d279-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2d279-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="2d279-134">応答</span><span class="sxs-lookup"><span data-stu-id="2d279-134">Response</span></span>
<span data-ttu-id="2d279-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2d279-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2d279-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2d279-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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