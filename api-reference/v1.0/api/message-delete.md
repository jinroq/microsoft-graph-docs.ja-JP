---
title: メッセージを削除する
description: 指定したユーザーのメールボックス内のメッセージを削除するか、メッセージの関係を削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b944cb586b7da4580cf8242b25275e7e70e518e7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275671"
---
# <a name="delete-message"></a><span data-ttu-id="04f25-103">メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="04f25-103">Delete message</span></span>

<span data-ttu-id="04f25-104">指定したユーザーのメールボックス内のメッセージを削除するか、メッセージの関係を削除します。</span><span class="sxs-lookup"><span data-stu-id="04f25-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="04f25-105">**メモ**回復可能なアイテム削除フォルダー ([既知のフォルダー名](../resources/mailfolder.md) `recoverableitemsdeletions`で表される) のアイテムを削除できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="04f25-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="04f25-106">詳細については、「[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)」および「[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04f25-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="04f25-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04f25-107">Permissions</span></span>
<span data-ttu-id="04f25-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04f25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04f25-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04f25-110">Permission type</span></span>      | <span data-ttu-id="04f25-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04f25-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04f25-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04f25-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04f25-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f25-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="04f25-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04f25-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04f25-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f25-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="04f25-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04f25-116">Application</span></span> | <span data-ttu-id="04f25-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f25-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="04f25-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04f25-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="04f25-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04f25-119">Request headers</span></span>
| <span data-ttu-id="04f25-120">名前</span><span class="sxs-lookup"><span data-stu-id="04f25-120">Name</span></span>       | <span data-ttu-id="04f25-121">型</span><span class="sxs-lookup"><span data-stu-id="04f25-121">Type</span></span> | <span data-ttu-id="04f25-122">説明</span><span class="sxs-lookup"><span data-stu-id="04f25-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04f25-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f25-123">Authorization</span></span>  | <span data-ttu-id="04f25-124">string</span><span class="sxs-lookup"><span data-stu-id="04f25-124">string</span></span>  | <span data-ttu-id="04f25-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04f25-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04f25-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04f25-127">Request body</span></span>
<span data-ttu-id="04f25-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04f25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04f25-129">応答</span><span class="sxs-lookup"><span data-stu-id="04f25-129">Response</span></span>

<span data-ttu-id="04f25-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="04f25-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04f25-132">例</span><span class="sxs-lookup"><span data-stu-id="04f25-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04f25-133">要求</span><span class="sxs-lookup"><span data-stu-id="04f25-133">Request</span></span>
<span data-ttu-id="04f25-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04f25-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="04f25-135">応答</span><span class="sxs-lookup"><span data-stu-id="04f25-135">Response</span></span>
<span data-ttu-id="04f25-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="04f25-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="04f25-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="04f25-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="04f25-138">C#</span><span class="sxs-lookup"><span data-stu-id="04f25-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04f25-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="04f25-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="04f25-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="04f25-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
