---
title: 学校をリストする
description: クラスが授業を受けている学校のリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2bd44ae1b320c1ec842a5de8f462ad880fa69295
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955398"
---
# <a name="list-schools"></a><span data-ttu-id="a74b1-103">学校をリストする</span><span class="sxs-lookup"><span data-stu-id="a74b1-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a74b1-104">クラスが授業を受けている学校のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a74b1-104">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="a74b1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a74b1-105">Permissions</span></span>
<span data-ttu-id="a74b1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a74b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a74b1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a74b1-108">Permission type</span></span>      | <span data-ttu-id="a74b1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a74b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a74b1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a74b1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a74b1-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a74b1-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a74b1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a74b1-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a74b1-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="a74b1-113">Not supported</span></span>  |
|<span data-ttu-id="a74b1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a74b1-114">Application</span></span> | <span data-ttu-id="a74b1-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a74b1-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a74b1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a74b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a74b1-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a74b1-117">Optional query parameters</span></span>
<span data-ttu-id="a74b1-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a74b1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a74b1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a74b1-119">Request headers</span></span>
| <span data-ttu-id="a74b1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a74b1-120">Header</span></span>       | <span data-ttu-id="a74b1-121">値</span><span class="sxs-lookup"><span data-stu-id="a74b1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a74b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a74b1-122">Authorization</span></span>  | <span data-ttu-id="a74b1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a74b1-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="a74b1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a74b1-125">Request body</span></span>
<span data-ttu-id="a74b1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a74b1-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a74b1-127">応答</span><span class="sxs-lookup"><span data-stu-id="a74b1-127">Response</span></span>
<span data-ttu-id="a74b1-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a74b1-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a74b1-129">例</span><span class="sxs-lookup"><span data-stu-id="a74b1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a74b1-130">要求</span><span class="sxs-lookup"><span data-stu-id="a74b1-130">Request</span></span>
<span data-ttu-id="a74b1-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a74b1-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a74b1-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a74b1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a74b1-133">C#</span><span class="sxs-lookup"><span data-stu-id="a74b1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a74b1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a74b1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a74b1-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="a74b1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a74b1-136">Java</span><span class="sxs-lookup"><span data-stu-id="a74b1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a74b1-137">応答</span><span class="sxs-lookup"><span data-stu-id="a74b1-137">Response</span></span>
<span data-ttu-id="a74b1-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a74b1-138">The following is an example of the response.</span></span> 

><span data-ttu-id="a74b1-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a74b1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
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
      "externalId": "10002",
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
