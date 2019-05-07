---
title: mailFolder を削除する
description: 指定した mailFolder を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1effb7d8e0ba6a27ddbef979f85c6e1e81adcecd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612645"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="55def-103">mailFolder を削除する</span><span class="sxs-lookup"><span data-stu-id="55def-103">Delete mailFolder</span></span>

<span data-ttu-id="55def-104">指定した[Mailfolder](../resources/mailfolder.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="55def-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="55def-105">メールフォルダーは、フォルダー ID または[既知のフォルダー名](../resources/mailfolder.md)(存在する場合) で指定できます。</span><span class="sxs-lookup"><span data-stu-id="55def-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="55def-106">**メモ**回復可能なアイテム削除フォルダー (既知のフォルダー名`recoverableitemsdeletions`で表される) のアイテムを削除できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="55def-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="55def-107">詳細については、「[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)」および「[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55def-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="55def-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="55def-108">Permissions</span></span>
<span data-ttu-id="55def-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55def-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55def-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55def-111">Permission type</span></span>      | <span data-ttu-id="55def-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="55def-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55def-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="55def-113">Delegated (work or school account)</span></span> | <span data-ttu-id="55def-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55def-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="55def-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55def-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55def-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55def-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="55def-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55def-117">Application</span></span> | <span data-ttu-id="55def-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55def-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="55def-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55def-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="55def-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55def-120">Request headers</span></span>
| <span data-ttu-id="55def-121">名前</span><span class="sxs-lookup"><span data-stu-id="55def-121">Name</span></span>       | <span data-ttu-id="55def-122">型</span><span class="sxs-lookup"><span data-stu-id="55def-122">Type</span></span> | <span data-ttu-id="55def-123">説明</span><span class="sxs-lookup"><span data-stu-id="55def-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55def-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="55def-124">Authorization</span></span>  | <span data-ttu-id="55def-125">string</span><span class="sxs-lookup"><span data-stu-id="55def-125">string</span></span>  | <span data-ttu-id="55def-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="55def-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55def-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="55def-128">Request body</span></span>
<span data-ttu-id="55def-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="55def-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55def-130">応答</span><span class="sxs-lookup"><span data-stu-id="55def-130">Response</span></span>

<span data-ttu-id="55def-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="55def-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55def-133">例</span><span class="sxs-lookup"><span data-stu-id="55def-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55def-134">要求</span><span class="sxs-lookup"><span data-stu-id="55def-134">Request</span></span>
<span data-ttu-id="55def-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="55def-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="55def-136">応答</span><span class="sxs-lookup"><span data-stu-id="55def-136">Response</span></span>
<span data-ttu-id="55def-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="55def-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="55def-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="55def-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="55def-139">Visual</span><span class="sxs-lookup"><span data-stu-id="55def-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55def-140">Java</span><span class="sxs-lookup"><span data-stu-id="55def-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
