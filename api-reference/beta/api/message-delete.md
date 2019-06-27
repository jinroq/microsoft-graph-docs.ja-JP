---
title: メッセージを削除する
description: 指定したユーザーのメールボックス内のメッセージを削除するか、メッセージの関係を削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d1df6b9d9b1b01d2960c12ce7cee1a927843626f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266088"
---
# <a name="delete-message"></a><span data-ttu-id="cbbc7-103">メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="cbbc7-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbbc7-104">指定したユーザーのメールボックス内のメッセージを削除するか、メッセージの関係を削除します。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="cbbc7-105">たとえば、メッセージ内の指定されたユーザーの特定の[@](../resources/mention.md)を削除することができます。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="cbbc7-106">**メモ**回復可能なアイテム削除フォルダー ([既知のフォルダー名](../resources/mailfolder.md) `recoverableitemsdeletions`で表される) のアイテムを削除できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="cbbc7-107">詳細については、「[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)」および「[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbbc7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cbbc7-108">Permissions</span></span>
<span data-ttu-id="cbbc7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbbc7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cbbc7-111">Permission type</span></span>      | <span data-ttu-id="cbbc7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cbbc7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbbc7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cbbc7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cbbc7-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbbc7-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cbbc7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cbbc7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbbc7-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbbc7-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cbbc7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cbbc7-117">Application</span></span> | <span data-ttu-id="cbbc7-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbbc7-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbbc7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cbbc7-119">HTTP request</span></span>

<span data-ttu-id="cbbc7-120">指定したメッセージを削除するには</span><span class="sxs-lookup"><span data-stu-id="cbbc7-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="cbbc7-121">メッセージ内の特定の[メンション](../resources/mention.md)を削除するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cbbc7-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbbc7-122">Request headers</span></span>
| <span data-ttu-id="cbbc7-123">名前</span><span class="sxs-lookup"><span data-stu-id="cbbc7-123">Name</span></span>       | <span data-ttu-id="cbbc7-124">型</span><span class="sxs-lookup"><span data-stu-id="cbbc7-124">Type</span></span> | <span data-ttu-id="cbbc7-125">説明</span><span class="sxs-lookup"><span data-stu-id="cbbc7-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cbbc7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbbc7-126">Authorization</span></span>  | <span data-ttu-id="cbbc7-127">string</span><span class="sxs-lookup"><span data-stu-id="cbbc7-127">string</span></span>  | <span data-ttu-id="cbbc7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbbc7-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="cbbc7-130">Request body</span></span>
<span data-ttu-id="cbbc7-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbbc7-132">応答</span><span class="sxs-lookup"><span data-stu-id="cbbc7-132">Response</span></span>

<span data-ttu-id="cbbc7-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbbc7-135">例</span><span class="sxs-lookup"><span data-stu-id="cbbc7-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="cbbc7-136">要求 1</span><span class="sxs-lookup"><span data-stu-id="cbbc7-136">Request 1</span></span>
<span data-ttu-id="cbbc7-137">最初の例では、指定したメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="cbbc7-138">応答 1</span><span class="sxs-lookup"><span data-stu-id="cbbc7-138">Response 1</span></span>
<span data-ttu-id="cbbc7-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cbbc7-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="cbbc7-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cbbc7-141">C#</span><span class="sxs-lookup"><span data-stu-id="cbbc7-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbbc7-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="cbbc7-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cbbc7-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="cbbc7-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="cbbc7-144">要求 2</span><span class="sxs-lookup"><span data-stu-id="cbbc7-144">Request 2</span></span>
<span data-ttu-id="cbbc7-145">次の例では、指定されたメッセージ内の特定の**メンション**を削除します。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-145">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="cbbc7-146">応答 2</span><span class="sxs-lookup"><span data-stu-id="cbbc7-146">Response 2</span></span>
<span data-ttu-id="cbbc7-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cbbc7-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cbbc7-148">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="cbbc7-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cbbc7-149">C#</span><span class="sxs-lookup"><span data-stu-id="cbbc7-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbbc7-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="cbbc7-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cbbc7-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="cbbc7-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
