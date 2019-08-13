---
title: mailFolder を削除する
description: 指定した mailFolder を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8b8ed2e0db5e22d5f068dfcc53e0ddb482ed5e4b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326633"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="fd1a4-103">mailFolder を削除する</span><span class="sxs-lookup"><span data-stu-id="fd1a4-103">Delete mailFolder</span></span>

<span data-ttu-id="fd1a4-104">指定した[Mailfolder](../resources/mailfolder.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="fd1a4-105">このフォルダーは、 [Mailsearchfolder](../resources/mailsearchfolder.md)にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-105">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="fd1a4-106">メールフォルダーは、フォルダー ID または[既知のフォルダー名](../resources/mailfolder.md)(存在する場合) で指定できます。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-106">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="fd1a4-107">**メモ**回復可能なアイテム削除フォルダー (既知のフォルダー名`recoverableitemsdeletions`で表される) のアイテムを削除できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="fd1a4-108">詳細については、「[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)」および「[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-108">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd1a4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd1a4-109">Permissions</span></span>
<span data-ttu-id="fd1a4-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd1a4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd1a4-112">Permission type</span></span>      | <span data-ttu-id="fd1a4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd1a4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd1a4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd1a4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fd1a4-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd1a4-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fd1a4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd1a4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd1a4-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd1a4-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fd1a4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd1a4-118">Application</span></span> | <span data-ttu-id="fd1a4-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd1a4-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd1a4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd1a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fd1a4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd1a4-121">Request headers</span></span>
| <span data-ttu-id="fd1a4-122">名前</span><span class="sxs-lookup"><span data-stu-id="fd1a4-122">Name</span></span>       | <span data-ttu-id="fd1a4-123">型</span><span class="sxs-lookup"><span data-stu-id="fd1a4-123">Type</span></span> | <span data-ttu-id="fd1a4-124">説明</span><span class="sxs-lookup"><span data-stu-id="fd1a4-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd1a4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd1a4-125">Authorization</span></span>  | <span data-ttu-id="fd1a4-126">string</span><span class="sxs-lookup"><span data-stu-id="fd1a4-126">string</span></span>  | <span data-ttu-id="fd1a4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd1a4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd1a4-129">Request body</span></span>
<span data-ttu-id="fd1a4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd1a4-131">応答</span><span class="sxs-lookup"><span data-stu-id="fd1a4-131">Response</span></span>

<span data-ttu-id="fd1a4-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd1a4-134">例</span><span class="sxs-lookup"><span data-stu-id="fd1a4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd1a4-135">要求</span><span class="sxs-lookup"><span data-stu-id="fd1a4-135">Request</span></span>
<span data-ttu-id="fd1a4-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fd1a4-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fd1a4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fd1a4-138">C#</span><span class="sxs-lookup"><span data-stu-id="fd1a4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd1a4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd1a4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fd1a4-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="fd1a4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fd1a4-141">Java</span><span class="sxs-lookup"><span data-stu-id="fd1a4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fd1a4-142">応答</span><span class="sxs-lookup"><span data-stu-id="fd1a4-142">Response</span></span>
<span data-ttu-id="fd1a4-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fd1a4-143">Here is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
