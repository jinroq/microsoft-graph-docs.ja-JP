---
title: educationClasses をリストする
description: 学校が所有するクラスのリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2b7a3fe74fdd8a2144b7b7087f252d83d3bf59f6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278170"
---
# <a name="list-educationclasses"></a><span data-ttu-id="d1506-103">educationClasses をリストする</span><span class="sxs-lookup"><span data-stu-id="d1506-103">List educationClasses</span></span>

<span data-ttu-id="d1506-104">学校が所有するクラスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d1506-104">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1506-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d1506-105">Permissions</span></span>
<span data-ttu-id="d1506-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1506-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1506-108">Permission type</span></span>      | <span data-ttu-id="d1506-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1506-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1506-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1506-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d1506-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d1506-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="d1506-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1506-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d1506-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1506-113">Not supported.</span></span>  |
|<span data-ttu-id="d1506-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1506-114">Application</span></span> | <span data-ttu-id="d1506-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1506-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d1506-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1506-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1506-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d1506-117">Optional query parameters</span></span>
<span data-ttu-id="d1506-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d1506-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1506-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1506-119">Request headers</span></span>
| <span data-ttu-id="d1506-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1506-120">Header</span></span>       | <span data-ttu-id="d1506-121">値</span><span class="sxs-lookup"><span data-stu-id="d1506-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1506-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1506-122">Authorization</span></span>  | <span data-ttu-id="d1506-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d1506-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1506-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1506-125">Request body</span></span>
<span data-ttu-id="d1506-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d1506-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d1506-127">応答</span><span class="sxs-lookup"><span data-stu-id="d1506-127">Response</span></span>
<span data-ttu-id="d1506-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d1506-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1506-129">例</span><span class="sxs-lookup"><span data-stu-id="d1506-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1506-130">要求</span><span class="sxs-lookup"><span data-stu-id="d1506-130">Request</span></span>
<span data-ttu-id="d1506-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d1506-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
##### <a name="response"></a><span data-ttu-id="d1506-132">応答</span><span class="sxs-lookup"><span data-stu-id="d1506-132">Response</span></span>
<span data-ttu-id="d1506-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d1506-133">The following is an example of the response.</span></span> 

><span data-ttu-id="d1506-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d1506-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1506-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d1506-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1506-137">C#</span><span class="sxs-lookup"><span data-stu-id="d1506-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_classes-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1506-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1506-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_classes-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d1506-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="d1506-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_classes-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationschool-list-classes.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationschool-list-classes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationschool-list-classes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
