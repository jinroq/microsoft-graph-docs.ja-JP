---
title: educationClass を削除する
description: クラスを削除します。 クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8cf2f9c33b3811dd30867f1370f4e67bec10a232
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955482"
---
# <a name="delete-educationclass"></a><span data-ttu-id="36231-104">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="36231-104">Delete educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36231-105">クラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="36231-105">Delete a class.</span></span> <span data-ttu-id="36231-106">クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。</span><span class="sxs-lookup"><span data-stu-id="36231-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="36231-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36231-107">Permissions</span></span>
<span data-ttu-id="36231-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36231-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36231-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36231-110">Permission type</span></span>      | <span data-ttu-id="36231-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36231-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36231-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36231-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="36231-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36231-113">Not supported.</span></span>  |
|<span data-ttu-id="36231-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36231-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="36231-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36231-115">Not supported.</span></span>  |
|<span data-ttu-id="36231-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36231-116">Application</span></span> | <span data-ttu-id="36231-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36231-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36231-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36231-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="36231-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36231-119">Request headers</span></span>
| <span data-ttu-id="36231-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36231-120">Header</span></span>       | <span data-ttu-id="36231-121">値</span><span class="sxs-lookup"><span data-stu-id="36231-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36231-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36231-122">Authorization</span></span>  | <span data-ttu-id="36231-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36231-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36231-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="36231-125">Request body</span></span>
<span data-ttu-id="36231-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="36231-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="36231-127">応答</span><span class="sxs-lookup"><span data-stu-id="36231-127">Response</span></span>
<span data-ttu-id="36231-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="36231-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36231-130">例</span><span class="sxs-lookup"><span data-stu-id="36231-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36231-131">要求</span><span class="sxs-lookup"><span data-stu-id="36231-131">Request</span></span>
<span data-ttu-id="36231-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36231-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36231-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="36231-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36231-134">C#</span><span class="sxs-lookup"><span data-stu-id="36231-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36231-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="36231-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36231-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="36231-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36231-137">Java</span><span class="sxs-lookup"><span data-stu-id="36231-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36231-138">応答</span><span class="sxs-lookup"><span data-stu-id="36231-138">Response</span></span>
<span data-ttu-id="36231-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36231-139">The following is an example of the response.</span></span> 

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
