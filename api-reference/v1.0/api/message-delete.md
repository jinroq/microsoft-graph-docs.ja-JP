---
title: メッセージを削除する
description: 指定したユーザーのメールボックス内のメッセージを削除するか、メッセージの関係を削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cb9e6fd563688fc422bcaf748d931daf97c74985
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565073"
---
# <a name="delete-message"></a><span data-ttu-id="3cc64-103">メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="3cc64-103">Delete message</span></span>

<span data-ttu-id="3cc64-104">指定したユーザーのメールボックス内のメッセージを削除するか、メッセージの関係を削除します。</span><span class="sxs-lookup"><span data-stu-id="3cc64-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="3cc64-105">**メモ**回復可能なアイテム削除フォルダー ([既知のフォルダー名](../resources/mailfolder.md) `recoverableitemsdeletions`で表される) のアイテムを削除できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="3cc64-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="3cc64-106">詳細については、「[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)」および「[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cc64-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cc64-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3cc64-107">Permissions</span></span>
<span data-ttu-id="3cc64-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cc64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cc64-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3cc64-110">Permission type</span></span>      | <span data-ttu-id="3cc64-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3cc64-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cc64-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3cc64-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3cc64-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cc64-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3cc64-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3cc64-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cc64-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cc64-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3cc64-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3cc64-116">Application</span></span> | <span data-ttu-id="3cc64-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cc64-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cc64-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3cc64-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3cc64-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cc64-119">Request headers</span></span>
| <span data-ttu-id="3cc64-120">名前</span><span class="sxs-lookup"><span data-stu-id="3cc64-120">Name</span></span>       | <span data-ttu-id="3cc64-121">型</span><span class="sxs-lookup"><span data-stu-id="3cc64-121">Type</span></span> | <span data-ttu-id="3cc64-122">説明</span><span class="sxs-lookup"><span data-stu-id="3cc64-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3cc64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cc64-123">Authorization</span></span>  | <span data-ttu-id="3cc64-124">string</span><span class="sxs-lookup"><span data-stu-id="3cc64-124">string</span></span>  | <span data-ttu-id="3cc64-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3cc64-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cc64-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3cc64-127">Request body</span></span>
<span data-ttu-id="3cc64-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3cc64-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cc64-129">応答</span><span class="sxs-lookup"><span data-stu-id="3cc64-129">Response</span></span>

<span data-ttu-id="3cc64-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3cc64-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cc64-132">例</span><span class="sxs-lookup"><span data-stu-id="3cc64-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cc64-133">要求</span><span class="sxs-lookup"><span data-stu-id="3cc64-133">Request</span></span>
<span data-ttu-id="3cc64-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3cc64-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="3cc64-135">応答</span><span class="sxs-lookup"><span data-stu-id="3cc64-135">Response</span></span>
<span data-ttu-id="3cc64-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3cc64-136">Here is an example of the response.</span></span> 
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
