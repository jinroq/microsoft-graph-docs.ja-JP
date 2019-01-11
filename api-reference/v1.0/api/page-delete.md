---
title: ページを削除する
description: OneNote のページを削除します。
localization_priority: Normal
ms.openlocfilehash: fc2a4a9e809cb3a335c795a27cb5ffe35487a880
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810011"
---
# <a name="delete-page"></a><span data-ttu-id="efcf9-103">ページを削除する</span><span class="sxs-lookup"><span data-stu-id="efcf9-103">Delete page</span></span>

<span data-ttu-id="efcf9-104">OneNote のページを削除します。</span><span class="sxs-lookup"><span data-stu-id="efcf9-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="efcf9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="efcf9-105">Permissions</span></span>
<span data-ttu-id="efcf9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efcf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efcf9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="efcf9-108">Permission type</span></span>      | <span data-ttu-id="efcf9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="efcf9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efcf9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="efcf9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="efcf9-111">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efcf9-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="efcf9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="efcf9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efcf9-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efcf9-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="efcf9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="efcf9-114">Application</span></span> | <span data-ttu-id="efcf9-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efcf9-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efcf9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="efcf9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="efcf9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="efcf9-117">Request headers</span></span>
| <span data-ttu-id="efcf9-118">名前</span><span class="sxs-lookup"><span data-stu-id="efcf9-118">Name</span></span>       | <span data-ttu-id="efcf9-119">種類</span><span class="sxs-lookup"><span data-stu-id="efcf9-119">Type</span></span> | <span data-ttu-id="efcf9-120">説明</span><span class="sxs-lookup"><span data-stu-id="efcf9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efcf9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="efcf9-121">Authorization</span></span>  | <span data-ttu-id="efcf9-122">string</span><span class="sxs-lookup"><span data-stu-id="efcf9-122">string</span></span>  | <span data-ttu-id="efcf9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="efcf9-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="efcf9-125">応答</span><span class="sxs-lookup"><span data-stu-id="efcf9-125">Response</span></span>

<span data-ttu-id="efcf9-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="efcf9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efcf9-128">例</span><span class="sxs-lookup"><span data-stu-id="efcf9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efcf9-129">要求</span><span class="sxs-lookup"><span data-stu-id="efcf9-129">Request</span></span>
<span data-ttu-id="efcf9-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="efcf9-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="efcf9-131">応答</span><span class="sxs-lookup"><span data-stu-id="efcf9-131">Response</span></span>
<span data-ttu-id="efcf9-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="efcf9-132">Here is an example of the response.</span></span>
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
