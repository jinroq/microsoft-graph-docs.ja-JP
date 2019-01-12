---
title: mailFolder を削除する
description: 指定した mailFolder または mailSearchFolder を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6753eaac9e02e5b6c5ff92402f13484dc458b558
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923867"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="7d991-103">mailFolder を削除する</span><span class="sxs-lookup"><span data-stu-id="7d991-103">Delete mailFolder</span></span>

> <span data-ttu-id="7d991-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d991-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d991-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d991-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d991-106">指定した[mailFolder](../resources/mailfolder.md)または[mailSearchFolder](../resources/mailsearchfolder.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7d991-106">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="7d991-107">いずれかが存在する場合、フォルダー id、または[よく知られているフォルダー名](../resources/mailfolder.md)、メールのフォルダーが存在することが可能です。</span><span class="sxs-lookup"><span data-stu-id="7d991-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="7d991-108">**メモ**回復可能なアイテムの削除フォルダー内のアイテムを削除できない場合があります (よく知られているフォルダー名で表される`recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="7d991-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="7d991-109">詳細については、[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)と[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d991-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d991-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d991-110">Permissions</span></span>
<span data-ttu-id="7d991-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d991-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d991-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d991-113">Permission type</span></span>      | <span data-ttu-id="7d991-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d991-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d991-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d991-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7d991-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d991-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7d991-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d991-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d991-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d991-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7d991-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d991-119">Application</span></span> | <span data-ttu-id="7d991-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d991-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d991-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d991-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7d991-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d991-122">Request headers</span></span>
| <span data-ttu-id="7d991-123">名前</span><span class="sxs-lookup"><span data-stu-id="7d991-123">Name</span></span>       | <span data-ttu-id="7d991-124">種類</span><span class="sxs-lookup"><span data-stu-id="7d991-124">Type</span></span> | <span data-ttu-id="7d991-125">説明</span><span class="sxs-lookup"><span data-stu-id="7d991-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d991-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d991-126">Authorization</span></span>  | <span data-ttu-id="7d991-127">string</span><span class="sxs-lookup"><span data-stu-id="7d991-127">string</span></span>  | <span data-ttu-id="7d991-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d991-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d991-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d991-130">Request body</span></span>
<span data-ttu-id="7d991-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7d991-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d991-132">応答</span><span class="sxs-lookup"><span data-stu-id="7d991-132">Response</span></span>
<span data-ttu-id="7d991-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7d991-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d991-135">例</span><span class="sxs-lookup"><span data-stu-id="7d991-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7d991-136">要求</span><span class="sxs-lookup"><span data-stu-id="7d991-136">Request</span></span>
<span data-ttu-id="7d991-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7d991-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="7d991-138">応答</span><span class="sxs-lookup"><span data-stu-id="7d991-138">Response</span></span>
<span data-ttu-id="7d991-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7d991-139">The following is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
