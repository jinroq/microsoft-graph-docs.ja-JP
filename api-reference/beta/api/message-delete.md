---
title: メッセージを削除する
description: 指定したユーザーのメールボックス内のメッセージを削除または、メッセージの関連付けを削除します。
localization_priority: Normal
ms.openlocfilehash: 3a76c936f72ebd238ee6d7a898dfd6a3e0356036
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864527"
---
# <a name="delete-message"></a><span data-ttu-id="6aaac-103">メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="6aaac-103">Delete message</span></span>

> <span data-ttu-id="6aaac-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6aaac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6aaac-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6aaac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6aaac-106">指定したユーザーのメールボックス内のメッセージを削除または、メッセージの関連付けを削除します。</span><span class="sxs-lookup"><span data-stu-id="6aaac-106">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="6aaac-107">たとえば、メッセージで指定したユーザーの特定の[言及 @](../resources/mention.md)を削除できます。</span><span class="sxs-lookup"><span data-stu-id="6aaac-107">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="6aaac-108">**メモ**回復可能なアイテムの削除フォルダー内のアイテムを削除できない場合があります ([よく知られているフォルダー名](../resources/mailfolder.md)で表される`recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="6aaac-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="6aaac-109">詳細については、[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)と[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aaac-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="6aaac-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6aaac-110">Permissions</span></span>
<span data-ttu-id="6aaac-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aaac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aaac-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6aaac-113">Permission type</span></span>      | <span data-ttu-id="6aaac-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6aaac-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6aaac-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6aaac-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6aaac-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6aaac-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6aaac-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6aaac-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aaac-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6aaac-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6aaac-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6aaac-119">Application</span></span> | <span data-ttu-id="6aaac-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6aaac-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aaac-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6aaac-121">HTTP request</span></span>

<span data-ttu-id="6aaac-122">指定したメッセージを削除します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6aaac-122">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="6aaac-123">特定[説明](../resources/mention.md)メッセージを削除します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6aaac-123">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6aaac-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6aaac-124">Request headers</span></span>
| <span data-ttu-id="6aaac-125">名前</span><span class="sxs-lookup"><span data-stu-id="6aaac-125">Name</span></span>       | <span data-ttu-id="6aaac-126">種類</span><span class="sxs-lookup"><span data-stu-id="6aaac-126">Type</span></span> | <span data-ttu-id="6aaac-127">説明</span><span class="sxs-lookup"><span data-stu-id="6aaac-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6aaac-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aaac-128">Authorization</span></span>  | <span data-ttu-id="6aaac-129">string</span><span class="sxs-lookup"><span data-stu-id="6aaac-129">string</span></span>  | <span data-ttu-id="6aaac-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6aaac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6aaac-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="6aaac-132">Request body</span></span>
<span data-ttu-id="6aaac-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6aaac-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aaac-134">応答</span><span class="sxs-lookup"><span data-stu-id="6aaac-134">Response</span></span>

<span data-ttu-id="6aaac-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6aaac-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aaac-137">例</span><span class="sxs-lookup"><span data-stu-id="6aaac-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6aaac-138">要求 1</span><span class="sxs-lookup"><span data-stu-id="6aaac-138">Request 1</span></span>
<span data-ttu-id="6aaac-139">最初の例では、指定したメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="6aaac-139">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="6aaac-140">応答 1</span><span class="sxs-lookup"><span data-stu-id="6aaac-140">Response 1</span></span>
<span data-ttu-id="6aaac-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6aaac-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="6aaac-142">要求 2</span><span class="sxs-lookup"><span data-stu-id="6aaac-142">Request 2</span></span>
<span data-ttu-id="6aaac-143">次の使用例は、特定**説明**で指定されたメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="6aaac-143">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="6aaac-144">応答 2</span><span class="sxs-lookup"><span data-stu-id="6aaac-144">Response 2</span></span>
<span data-ttu-id="6aaac-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6aaac-145">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
