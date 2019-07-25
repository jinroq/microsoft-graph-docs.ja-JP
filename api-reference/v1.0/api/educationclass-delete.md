---
title: educationClass を削除する
description: クラスを削除します。 クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: cb901c2cee42203292a417d35fdb038264c1c29c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888411"
---
# <a name="delete-educationclass"></a><span data-ttu-id="e00fb-104">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="e00fb-104">Delete educationClass</span></span>

<span data-ttu-id="e00fb-105">クラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="e00fb-105">Delete a class.</span></span> <span data-ttu-id="e00fb-106">クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。</span><span class="sxs-lookup"><span data-stu-id="e00fb-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="e00fb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e00fb-107">Permissions</span></span>
<span data-ttu-id="e00fb-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e00fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e00fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e00fb-110">Permission type</span></span>      | <span data-ttu-id="e00fb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e00fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e00fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e00fb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e00fb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e00fb-113">Not supported.</span></span>  |
|<span data-ttu-id="e00fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e00fb-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e00fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e00fb-115">Not supported.</span></span>  |
|<span data-ttu-id="e00fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e00fb-116">Application</span></span> | <span data-ttu-id="e00fb-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e00fb-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e00fb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e00fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e00fb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e00fb-119">Request headers</span></span>
| <span data-ttu-id="e00fb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e00fb-120">Header</span></span>       | <span data-ttu-id="e00fb-121">値</span><span class="sxs-lookup"><span data-stu-id="e00fb-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e00fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e00fb-122">Authorization</span></span>  | <span data-ttu-id="e00fb-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e00fb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e00fb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e00fb-125">Request body</span></span>
<span data-ttu-id="e00fb-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e00fb-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e00fb-127">応答</span><span class="sxs-lookup"><span data-stu-id="e00fb-127">Response</span></span>
<span data-ttu-id="e00fb-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e00fb-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e00fb-130">例</span><span class="sxs-lookup"><span data-stu-id="e00fb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e00fb-131">要求</span><span class="sxs-lookup"><span data-stu-id="e00fb-131">Request</span></span>
<span data-ttu-id="e00fb-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e00fb-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e00fb-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e00fb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e00fb-134">C#</span><span class="sxs-lookup"><span data-stu-id="e00fb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e00fb-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e00fb-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e00fb-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="e00fb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e00fb-137">Java</span><span class="sxs-lookup"><span data-stu-id="e00fb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e00fb-138">応答</span><span class="sxs-lookup"><span data-stu-id="e00fb-138">Response</span></span>
<span data-ttu-id="e00fb-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e00fb-139">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
