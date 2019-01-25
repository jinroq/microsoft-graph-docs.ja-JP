---
title: mailFolder を削除する
description: 指定した mailFolder または mailSearchFolder を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e993d4cb770db546a11e80aa9b9fe24501e2b281
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512998"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="06a4e-103">mailFolder を削除する</span><span class="sxs-lookup"><span data-stu-id="06a4e-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06a4e-104">指定した[mailFolder](../resources/mailfolder.md)または[mailSearchFolder](../resources/mailsearchfolder.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-104">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="06a4e-105">いずれかが存在する場合、フォルダー id、または[よく知られているフォルダー名](../resources/mailfolder.md)、メールのフォルダーが存在することが可能です。</span><span class="sxs-lookup"><span data-stu-id="06a4e-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="06a4e-106">**メモ**回復可能なアイテムの削除フォルダー内のアイテムを削除できない場合があります (よく知られているフォルダー名で表される`recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="06a4e-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="06a4e-107">詳細については、[削除済みアイテムの保存期間](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)と[削除済みアイテムのクリーンアップ](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06a4e-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="06a4e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="06a4e-108">Permissions</span></span>
<span data-ttu-id="06a4e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06a4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06a4e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06a4e-111">Permission type</span></span>      | <span data-ttu-id="06a4e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="06a4e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06a4e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06a4e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="06a4e-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06a4e-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="06a4e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06a4e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06a4e-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06a4e-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="06a4e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06a4e-117">Application</span></span> | <span data-ttu-id="06a4e-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06a4e-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="06a4e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06a4e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="06a4e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06a4e-120">Request headers</span></span>
| <span data-ttu-id="06a4e-121">名前</span><span class="sxs-lookup"><span data-stu-id="06a4e-121">Name</span></span>       | <span data-ttu-id="06a4e-122">型</span><span class="sxs-lookup"><span data-stu-id="06a4e-122">Type</span></span> | <span data-ttu-id="06a4e-123">説明</span><span class="sxs-lookup"><span data-stu-id="06a4e-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="06a4e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="06a4e-124">Authorization</span></span>  | <span data-ttu-id="06a4e-125">string</span><span class="sxs-lookup"><span data-stu-id="06a4e-125">string</span></span>  | <span data-ttu-id="06a4e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="06a4e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06a4e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="06a4e-128">Request body</span></span>
<span data-ttu-id="06a4e-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="06a4e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06a4e-130">応答</span><span class="sxs-lookup"><span data-stu-id="06a4e-130">Response</span></span>
<span data-ttu-id="06a4e-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="06a4e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06a4e-133">例</span><span class="sxs-lookup"><span data-stu-id="06a4e-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="06a4e-134">要求</span><span class="sxs-lookup"><span data-stu-id="06a4e-134">Request</span></span>
<span data-ttu-id="06a4e-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="06a4e-136">応答</span><span class="sxs-lookup"><span data-stu-id="06a4e-136">Response</span></span>
<span data-ttu-id="06a4e-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-137">The following is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
