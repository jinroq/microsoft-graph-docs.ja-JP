---
title: メッセージを削除する
description: 指定したユーザーのメールボックス内のメッセージを削除または、メッセージの関連付けを削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1237ba7e4aa5ab0439af9f07902705e7b4061374
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513544"
---
# <a name="delete-message"></a><span data-ttu-id="35aa3-103">メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="35aa3-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35aa3-104">指定したユーザーのメールボックス内のメッセージを削除または、メッセージの関連付けを削除します。</span><span class="sxs-lookup"><span data-stu-id="35aa3-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="35aa3-105">たとえば、メッセージで指定したユーザーの特定の[言及 @](../resources/mention.md)を削除できます。</span><span class="sxs-lookup"><span data-stu-id="35aa3-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="35aa3-106">**メモ**回復可能なアイテムの削除フォルダー内のアイテムを削除できない場合があります ([よく知られているフォルダー名](../resources/mailfolder.md)で表される`recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="35aa3-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="35aa3-107">詳細については、[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)と[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35aa3-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="35aa3-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="35aa3-108">Permissions</span></span>
<span data-ttu-id="35aa3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35aa3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35aa3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35aa3-111">Permission type</span></span>      | <span data-ttu-id="35aa3-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="35aa3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35aa3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35aa3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="35aa3-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35aa3-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35aa3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35aa3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35aa3-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35aa3-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35aa3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35aa3-117">Application</span></span> | <span data-ttu-id="35aa3-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35aa3-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35aa3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35aa3-119">HTTP request</span></span>

<span data-ttu-id="35aa3-120">指定したメッセージを削除します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="35aa3-120">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="35aa3-121">特定[説明](../resources/mention.md)メッセージを削除します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="35aa3-121">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35aa3-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35aa3-122">Request headers</span></span>
| <span data-ttu-id="35aa3-123">名前</span><span class="sxs-lookup"><span data-stu-id="35aa3-123">Name</span></span>       | <span data-ttu-id="35aa3-124">型</span><span class="sxs-lookup"><span data-stu-id="35aa3-124">Type</span></span> | <span data-ttu-id="35aa3-125">説明</span><span class="sxs-lookup"><span data-stu-id="35aa3-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="35aa3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="35aa3-126">Authorization</span></span>  | <span data-ttu-id="35aa3-127">string</span><span class="sxs-lookup"><span data-stu-id="35aa3-127">string</span></span>  | <span data-ttu-id="35aa3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="35aa3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35aa3-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="35aa3-130">Request body</span></span>
<span data-ttu-id="35aa3-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="35aa3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35aa3-132">応答</span><span class="sxs-lookup"><span data-stu-id="35aa3-132">Response</span></span>

<span data-ttu-id="35aa3-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="35aa3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35aa3-135">例</span><span class="sxs-lookup"><span data-stu-id="35aa3-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="35aa3-136">要求 1</span><span class="sxs-lookup"><span data-stu-id="35aa3-136">Request 1</span></span>
<span data-ttu-id="35aa3-137">最初の例では、指定したメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="35aa3-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="35aa3-138">応答 1</span><span class="sxs-lookup"><span data-stu-id="35aa3-138">Response 1</span></span>
<span data-ttu-id="35aa3-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="35aa3-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="35aa3-140">要求 2</span><span class="sxs-lookup"><span data-stu-id="35aa3-140">Request 2</span></span>
<span data-ttu-id="35aa3-141">次の使用例は、特定**説明**で指定されたメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="35aa3-141">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="35aa3-142">応答 2</span><span class="sxs-lookup"><span data-stu-id="35aa3-142">Response 2</span></span>
<span data-ttu-id="35aa3-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="35aa3-143">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
