---
title: OutlookTaskFolder の削除
description: 指定された Outlook タスクフォルダーを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 647664bd2bde173fe5ffaf624cfc353736540df3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447251"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="5a3b7-103">OutlookTaskFolder の削除</span><span class="sxs-lookup"><span data-stu-id="5a3b7-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a3b7-104">指定された Outlook タスクフォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="5a3b7-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a3b7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a3b7-105">Permissions</span></span>
<span data-ttu-id="5a3b7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a3b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a3b7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a3b7-108">Permission type</span></span>      | <span data-ttu-id="5a3b7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a3b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a3b7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a3b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a3b7-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a3b7-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5a3b7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a3b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a3b7-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a3b7-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5a3b7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a3b7-114">Application</span></span> | <span data-ttu-id="5a3b7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a3b7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a3b7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a3b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5a3b7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a3b7-117">Request headers</span></span>
| <span data-ttu-id="5a3b7-118">名前</span><span class="sxs-lookup"><span data-stu-id="5a3b7-118">Name</span></span>       | <span data-ttu-id="5a3b7-119">説明</span><span class="sxs-lookup"><span data-stu-id="5a3b7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5a3b7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a3b7-120">Authorization</span></span>  | <span data-ttu-id="5a3b7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a3b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a3b7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a3b7-123">Request body</span></span>
<span data-ttu-id="5a3b7-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5a3b7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a3b7-125">応答</span><span class="sxs-lookup"><span data-stu-id="5a3b7-125">Response</span></span>

<span data-ttu-id="5a3b7-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5a3b7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a3b7-128">例</span><span class="sxs-lookup"><span data-stu-id="5a3b7-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a3b7-129">要求</span><span class="sxs-lookup"><span data-stu-id="5a3b7-129">Request</span></span>
<span data-ttu-id="5a3b7-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5a3b7-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5a3b7-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5a3b7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5a3b7-132">C#</span><span class="sxs-lookup"><span data-stu-id="5a3b7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a3b7-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="5a3b7-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a3b7-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="5a3b7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5a3b7-135">応答</span><span class="sxs-lookup"><span data-stu-id="5a3b7-135">Response</span></span>
<span data-ttu-id="5a3b7-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5a3b7-136">Here is an example of the response.</span></span> 
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
  "description": "Delete outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
