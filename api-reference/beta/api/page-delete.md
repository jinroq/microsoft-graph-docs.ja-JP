---
title: ページを削除する
description: OneNote のページを削除します。
ms.openlocfilehash: f2e566696937ee6f7808a66f994298802be66a17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067977"
---
# <a name="delete-page"></a><span data-ttu-id="18b61-103">ページを削除する</span><span class="sxs-lookup"><span data-stu-id="18b61-103">Delete page</span></span>

> <span data-ttu-id="18b61-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18b61-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18b61-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b61-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18b61-106">OneNote のページを削除します。</span><span class="sxs-lookup"><span data-stu-id="18b61-106">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="18b61-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18b61-107">Permissions</span></span>
<span data-ttu-id="18b61-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18b61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18b61-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18b61-110">Permission type</span></span>      | <span data-ttu-id="18b61-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18b61-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18b61-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18b61-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18b61-113">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b61-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="18b61-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18b61-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18b61-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18b61-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="18b61-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18b61-116">Application</span></span> | <span data-ttu-id="18b61-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b61-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18b61-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18b61-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="18b61-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18b61-119">Request headers</span></span>
| <span data-ttu-id="18b61-120">名前</span><span class="sxs-lookup"><span data-stu-id="18b61-120">Name</span></span>       | <span data-ttu-id="18b61-121">型</span><span class="sxs-lookup"><span data-stu-id="18b61-121">Type</span></span> | <span data-ttu-id="18b61-122">説明</span><span class="sxs-lookup"><span data-stu-id="18b61-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18b61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b61-123">Authorization</span></span>  | <span data-ttu-id="18b61-124">string</span><span class="sxs-lookup"><span data-stu-id="18b61-124">string</span></span>  | <span data-ttu-id="18b61-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18b61-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="18b61-127">応答</span><span class="sxs-lookup"><span data-stu-id="18b61-127">Response</span></span>

<span data-ttu-id="18b61-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="18b61-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b61-130">例</span><span class="sxs-lookup"><span data-stu-id="18b61-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18b61-131">要求</span><span class="sxs-lookup"><span data-stu-id="18b61-131">Request</span></span>
<span data-ttu-id="18b61-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18b61-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="18b61-133">応答</span><span class="sxs-lookup"><span data-stu-id="18b61-133">Response</span></span>
<span data-ttu-id="18b61-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="18b61-134">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->