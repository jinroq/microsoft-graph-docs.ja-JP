---
title: educationSchool を取得する
description: 学校オブジェクトのプロパティと関係を取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5ece296d66d2614e3c53b5d0f3bd47de17114807
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416164"
---
# <a name="get-educationschool"></a><span data-ttu-id="e6fc4-103">educationSchool を取得する</span><span class="sxs-lookup"><span data-stu-id="e6fc4-103">Get educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6fc4-104">学校オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6fc4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e6fc4-105">Permissions</span></span>
<span data-ttu-id="e6fc4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6fc4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6fc4-108">Permission type</span></span>      | <span data-ttu-id="e6fc4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6fc4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6fc4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6fc4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6fc4-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e6fc4-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="e6fc4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6fc4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e6fc4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-113">Not supported.</span></span>  |
|<span data-ttu-id="e6fc4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6fc4-114">Application</span></span> | <span data-ttu-id="e6fc4-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6fc4-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e6fc4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6fc4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6fc4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e6fc4-117">Optional query parameters</span></span>
<span data-ttu-id="e6fc4-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6fc4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6fc4-119">Request headers</span></span>
| <span data-ttu-id="e6fc4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6fc4-120">Header</span></span>       | <span data-ttu-id="e6fc4-121">値</span><span class="sxs-lookup"><span data-stu-id="e6fc4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6fc4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6fc4-122">Authorization</span></span>  | <span data-ttu-id="e6fc4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6fc4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6fc4-125">Request body</span></span>
<span data-ttu-id="e6fc4-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e6fc4-127">応答</span><span class="sxs-lookup"><span data-stu-id="e6fc4-127">Response</span></span>
<span data-ttu-id="e6fc4-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6fc4-129">例</span><span class="sxs-lookup"><span data-stu-id="e6fc4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6fc4-130">要求</span><span class="sxs-lookup"><span data-stu-id="e6fc4-130">Request</span></span>
<span data-ttu-id="e6fc4-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e6fc4-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e6fc4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10001
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e6fc4-133">C#</span><span class="sxs-lookup"><span data-stu-id="e6fc4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6fc4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6fc4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e6fc4-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="e6fc4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e6fc4-136">応答</span><span class="sxs-lookup"><span data-stu-id="e6fc4-136">Response</span></span>
<span data-ttu-id="e6fc4-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-137">The following is an example of the response.</span></span> 

><span data-ttu-id="e6fc4-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e6fc4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "schoolPrincipalEmail": "AmyRoebuck@contoso.com",
  "schoolPrincipalName": "Amy Roebuck",
  "externalSchoolPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
