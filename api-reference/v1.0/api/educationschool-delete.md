---
title: educationSchool を削除する
description: 学校を削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b7c3bfe0d2a99fe7fe72e6d6303e66d81191650a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445199"
---
# <a name="delete-educationschool"></a><span data-ttu-id="ce82a-103">educationSchool を削除する</span><span class="sxs-lookup"><span data-stu-id="ce82a-103">Delete educationSchool</span></span>

<span data-ttu-id="ce82a-104">学校を削除します。</span><span class="sxs-lookup"><span data-stu-id="ce82a-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce82a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce82a-105">Permissions</span></span>
<span data-ttu-id="ce82a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce82a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce82a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce82a-108">Permission type</span></span>      | <span data-ttu-id="ce82a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce82a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce82a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce82a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ce82a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce82a-111">Not supported.</span></span>  |
|<span data-ttu-id="ce82a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce82a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ce82a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce82a-113">Not supported.</span></span>  |
|<span data-ttu-id="ce82a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce82a-114">Application</span></span> | <span data-ttu-id="ce82a-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce82a-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ce82a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce82a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ce82a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce82a-117">Request headers</span></span>
| <span data-ttu-id="ce82a-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce82a-118">Header</span></span>       | <span data-ttu-id="ce82a-119">値</span><span class="sxs-lookup"><span data-stu-id="ce82a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce82a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce82a-120">Authorization</span></span>  | <span data-ttu-id="ce82a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce82a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce82a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce82a-123">Request body</span></span>
<span data-ttu-id="ce82a-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce82a-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ce82a-125">応答</span><span class="sxs-lookup"><span data-stu-id="ce82a-125">Response</span></span>
<span data-ttu-id="ce82a-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ce82a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce82a-128">例</span><span class="sxs-lookup"><span data-stu-id="ce82a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce82a-129">要求</span><span class="sxs-lookup"><span data-stu-id="ce82a-129">Request</span></span>
<span data-ttu-id="ce82a-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce82a-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ce82a-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ce82a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce82a-132">C#</span><span class="sxs-lookup"><span data-stu-id="ce82a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce82a-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce82a-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce82a-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="ce82a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ce82a-135">応答</span><span class="sxs-lookup"><span data-stu-id="ce82a-135">Response</span></span>
<span data-ttu-id="ce82a-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce82a-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
