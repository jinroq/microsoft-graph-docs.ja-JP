---
title: educationSchool を削除する
description: 学校を削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 337bc03df9aec93bdcbfebc84db3467bf8748342
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955202"
---
# <a name="delete-educationschool"></a><span data-ttu-id="903da-103">educationSchool を削除する</span><span class="sxs-lookup"><span data-stu-id="903da-103">Delete educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="903da-104">学校を削除します。</span><span class="sxs-lookup"><span data-stu-id="903da-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="903da-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="903da-105">Permissions</span></span>
<span data-ttu-id="903da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="903da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="903da-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="903da-108">Permission type</span></span>      | <span data-ttu-id="903da-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="903da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="903da-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="903da-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="903da-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="903da-111">Not supported.</span></span>  |
|<span data-ttu-id="903da-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="903da-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="903da-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="903da-113">Not supported.</span></span>  |
|<span data-ttu-id="903da-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="903da-114">Application</span></span> | <span data-ttu-id="903da-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="903da-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="903da-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="903da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="903da-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="903da-117">Request headers</span></span>
| <span data-ttu-id="903da-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="903da-118">Header</span></span>       | <span data-ttu-id="903da-119">値</span><span class="sxs-lookup"><span data-stu-id="903da-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="903da-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="903da-120">Authorization</span></span>  | <span data-ttu-id="903da-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="903da-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="903da-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="903da-123">Request body</span></span>
<span data-ttu-id="903da-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="903da-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="903da-125">応答</span><span class="sxs-lookup"><span data-stu-id="903da-125">Response</span></span>
<span data-ttu-id="903da-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="903da-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="903da-128">例</span><span class="sxs-lookup"><span data-stu-id="903da-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="903da-129">要求</span><span class="sxs-lookup"><span data-stu-id="903da-129">Request</span></span>
<span data-ttu-id="903da-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="903da-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="903da-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="903da-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="903da-132">C#</span><span class="sxs-lookup"><span data-stu-id="903da-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="903da-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="903da-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="903da-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="903da-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="903da-135">Java</span><span class="sxs-lookup"><span data-stu-id="903da-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="903da-136">応答</span><span class="sxs-lookup"><span data-stu-id="903da-136">Response</span></span>
<span data-ttu-id="903da-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="903da-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
