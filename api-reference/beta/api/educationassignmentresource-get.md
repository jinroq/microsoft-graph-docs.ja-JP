---
title: EducationAssignmentResource を取得する
description: '割り当ての特定のリソースのプロパティを取得します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1d982092d35ae12aa660bce9c9a9e229395b6df1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860708"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="e3b38-103">EducationAssignmentResource を取得する</span><span class="sxs-lookup"><span data-stu-id="e3b38-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3b38-104">割り当ての特定のリソースのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3b38-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="e3b38-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3b38-105">Permissions</span></span>
<span data-ttu-id="e3b38-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3b38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3b38-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3b38-108">Permission type</span></span>      | <span data-ttu-id="e3b38-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3b38-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3b38-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3b38-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e3b38-111">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="e3b38-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="e3b38-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3b38-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e3b38-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3b38-113">Not supported.</span></span>  |
|<span data-ttu-id="e3b38-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3b38-114">Application</span></span> |  <span data-ttu-id="e3b38-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3b38-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e3b38-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3b38-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3b38-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3b38-117">Optional query parameters</span></span>
<span data-ttu-id="e3b38-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3b38-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3b38-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3b38-119">Request headers</span></span>
| <span data-ttu-id="e3b38-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3b38-120">Header</span></span>       | <span data-ttu-id="e3b38-121">値</span><span class="sxs-lookup"><span data-stu-id="e3b38-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3b38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3b38-122">Authorization</span></span>  | <span data-ttu-id="e3b38-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3b38-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3b38-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3b38-125">Request body</span></span>
<span data-ttu-id="e3b38-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e3b38-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e3b38-127">応答</span><span class="sxs-lookup"><span data-stu-id="e3b38-127">Response</span></span>
<span data-ttu-id="e3b38-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3b38-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3b38-129">例</span><span class="sxs-lookup"><span data-stu-id="e3b38-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3b38-130">要求</span><span class="sxs-lookup"><span data-stu-id="e3b38-130">Request</span></span>
<span data-ttu-id="e3b38-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3b38-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e3b38-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e3b38-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3b38-133">C#</span><span class="sxs-lookup"><span data-stu-id="e3b38-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3b38-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3b38-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3b38-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="e3b38-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e3b38-136">Java</span><span class="sxs-lookup"><span data-stu-id="e3b38-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e3b38-137">応答</span><span class="sxs-lookup"><span data-stu-id="e3b38-137">Response</span></span>
<span data-ttu-id="e3b38-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3b38-138">The following is an example of the response.</span></span> 

><span data-ttu-id="e3b38-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e3b38-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e3b38-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e3b38-140">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
