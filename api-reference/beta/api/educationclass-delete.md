---
title: educationClass を削除する
description: クラスを削除します。 クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f94a1f5bf7fdf935e00ae760f0f5d2601b89276d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416458"
---
# <a name="delete-educationclass"></a><span data-ttu-id="3b756-104">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="3b756-104">Delete educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b756-105">クラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="3b756-105">Delete a class.</span></span> <span data-ttu-id="3b756-106">クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。</span><span class="sxs-lookup"><span data-stu-id="3b756-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b756-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b756-107">Permissions</span></span>
<span data-ttu-id="3b756-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b756-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b756-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b756-110">Permission type</span></span>      | <span data-ttu-id="3b756-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b756-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b756-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b756-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3b756-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b756-113">Not supported.</span></span>  |
|<span data-ttu-id="3b756-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b756-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3b756-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b756-115">Not supported.</span></span>  |
|<span data-ttu-id="3b756-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b756-116">Application</span></span> | <span data-ttu-id="3b756-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b756-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3b756-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b756-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3b756-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b756-119">Request headers</span></span>
| <span data-ttu-id="3b756-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b756-120">Header</span></span>       | <span data-ttu-id="3b756-121">値</span><span class="sxs-lookup"><span data-stu-id="3b756-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b756-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b756-122">Authorization</span></span>  | <span data-ttu-id="3b756-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b756-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b756-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b756-125">Request body</span></span>
<span data-ttu-id="3b756-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b756-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3b756-127">応答</span><span class="sxs-lookup"><span data-stu-id="3b756-127">Response</span></span>
<span data-ttu-id="3b756-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3b756-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b756-130">例</span><span class="sxs-lookup"><span data-stu-id="3b756-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b756-131">要求</span><span class="sxs-lookup"><span data-stu-id="3b756-131">Request</span></span>
<span data-ttu-id="3b756-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3b756-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3b756-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3b756-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b756-134">C#</span><span class="sxs-lookup"><span data-stu-id="3b756-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b756-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b756-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b756-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="3b756-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3b756-137">応答</span><span class="sxs-lookup"><span data-stu-id="3b756-137">Response</span></span>
<span data-ttu-id="3b756-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3b756-138">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
