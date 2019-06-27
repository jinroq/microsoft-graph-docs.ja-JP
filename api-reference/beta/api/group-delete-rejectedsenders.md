---
title: rejectedSender の削除
description: 拒否された送信者の一覧からユーザーまたはグループを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ef3e1dd0e6280200d789c11659cd7d2ecd0f80ce
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263315"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="92434-103">rejectedSender の削除</span><span class="sxs-lookup"><span data-stu-id="92434-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92434-104">指定したグループの拒否リストからユーザーまたはグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="92434-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="92434-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="92434-105">Permissions</span></span>
<span data-ttu-id="92434-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92434-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92434-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92434-108">Permission type</span></span>                        | <span data-ttu-id="92434-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="92434-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="92434-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92434-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="92434-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92434-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="92434-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92434-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92434-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92434-113">Not supported.</span></span> |
| <span data-ttu-id="92434-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92434-114">Application</span></span>                            | <span data-ttu-id="92434-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92434-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92434-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92434-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="92434-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92434-117">Request headers</span></span>

| <span data-ttu-id="92434-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92434-118">Header</span></span>         | <span data-ttu-id="92434-119">値</span><span class="sxs-lookup"><span data-stu-id="92434-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="92434-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="92434-120">Authorization</span></span>  | <span data-ttu-id="92434-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="92434-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="92434-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="92434-123">Request body</span></span>
<span data-ttu-id="92434-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="92434-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92434-125">応答</span><span class="sxs-lookup"><span data-stu-id="92434-125">Response</span></span>
<span data-ttu-id="92434-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="92434-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92434-128">例</span><span class="sxs-lookup"><span data-stu-id="92434-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="92434-129">例 1: グループの拒否された送信者の一覧からユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="92434-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="92434-130">要求</span><span class="sxs-lookup"><span data-stu-id="92434-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
#### <a name="response"></a><span data-ttu-id="92434-131">応答</span><span class="sxs-lookup"><span data-stu-id="92434-131">Response</span></span>
<span data-ttu-id="92434-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="92434-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="92434-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="92434-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="92434-134">C#</span><span class="sxs-lookup"><span data-stu-id="92434-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92434-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="92434-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="92434-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="92434-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="92434-137">例 2: グループの拒否された送信者の一覧からグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="92434-137">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="92434-138">要求</span><span class="sxs-lookup"><span data-stu-id="92434-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="92434-139">応答</span><span class="sxs-lookup"><span data-stu-id="92434-139">Response</span></span>
<span data-ttu-id="92434-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="92434-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="92434-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="92434-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="92434-142">C#</span><span class="sxs-lookup"><span data-stu-id="92434-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92434-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="92434-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="92434-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="92434-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
