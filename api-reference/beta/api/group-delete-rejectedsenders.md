---
title: rejectedSender の削除
description: 拒否された送信者の一覧からユーザーまたはグループを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 8050be767bb2950eb1ebaf6d41a4c0b7c18c1270
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440639"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="0fd2c-103">rejectedSender の削除</span><span class="sxs-lookup"><span data-stu-id="0fd2c-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fd2c-104">指定したグループの拒否リストからユーザーまたはグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fd2c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0fd2c-105">Permissions</span></span>
<span data-ttu-id="0fd2c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fd2c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0fd2c-108">Permission type</span></span>                        | <span data-ttu-id="0fd2c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0fd2c-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="0fd2c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0fd2c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fd2c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fd2c-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="0fd2c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0fd2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fd2c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-113">Not supported.</span></span> |
| <span data-ttu-id="0fd2c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0fd2c-114">Application</span></span>                            | <span data-ttu-id="0fd2c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fd2c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fd2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="0fd2c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fd2c-117">Request headers</span></span>

| <span data-ttu-id="0fd2c-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fd2c-118">Header</span></span>         | <span data-ttu-id="0fd2c-119">値</span><span class="sxs-lookup"><span data-stu-id="0fd2c-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="0fd2c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fd2c-120">Authorization</span></span>  | <span data-ttu-id="0fd2c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="0fd2c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0fd2c-123">Request body</span></span>
<span data-ttu-id="0fd2c-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fd2c-125">応答</span><span class="sxs-lookup"><span data-stu-id="0fd2c-125">Response</span></span>
<span data-ttu-id="0fd2c-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fd2c-128">例</span><span class="sxs-lookup"><span data-stu-id="0fd2c-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="0fd2c-129">例 1: グループの拒否された送信者の一覧からユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="0fd2c-130">要求</span><span class="sxs-lookup"><span data-stu-id="0fd2c-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0fd2c-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0fd2c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fd2c-132">C#</span><span class="sxs-lookup"><span data-stu-id="0fd2c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fd2c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="0fd2c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fd2c-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="0fd2c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0fd2c-135">応答</span><span class="sxs-lookup"><span data-stu-id="0fd2c-135">Response</span></span>
<span data-ttu-id="0fd2c-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="0fd2c-137">例 2: グループの拒否された送信者の一覧からグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-137">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="0fd2c-138">要求</span><span class="sxs-lookup"><span data-stu-id="0fd2c-138">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0fd2c-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0fd2c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fd2c-140">C#</span><span class="sxs-lookup"><span data-stu-id="0fd2c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fd2c-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="0fd2c-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fd2c-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="0fd2c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0fd2c-143">応答</span><span class="sxs-lookup"><span data-stu-id="0fd2c-143">Response</span></span>
<span data-ttu-id="0fd2c-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fd2c-144">The following is an example of the response.</span></span> 
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
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
