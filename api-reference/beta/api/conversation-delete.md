---
title: Delete conversation
description: 会話を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7fc4c8d1d3f32cce54ae99687f23e5543be50017
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591232"
---
# <a name="delete-conversation"></a><span data-ttu-id="26ef5-103">Delete conversation</span><span class="sxs-lookup"><span data-stu-id="26ef5-103">Delete conversation</span></span>

<span data-ttu-id="26ef5-104">会話を削除します。</span><span class="sxs-lookup"><span data-stu-id="26ef5-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="26ef5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26ef5-105">Permissions</span></span>
<span data-ttu-id="26ef5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26ef5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26ef5-108">Permission type</span></span>      | <span data-ttu-id="26ef5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26ef5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26ef5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26ef5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="26ef5-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ef5-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="26ef5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26ef5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26ef5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26ef5-113">Not supported.</span></span>    |
|<span data-ttu-id="26ef5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26ef5-114">Application</span></span> | <span data-ttu-id="26ef5-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ef5-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26ef5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26ef5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="26ef5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26ef5-117">Request headers</span></span>
| <span data-ttu-id="26ef5-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26ef5-118">Header</span></span>       | <span data-ttu-id="26ef5-119">値</span><span class="sxs-lookup"><span data-stu-id="26ef5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26ef5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="26ef5-120">Authorization</span></span>  | <span data-ttu-id="26ef5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26ef5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26ef5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="26ef5-123">Request body</span></span>
<span data-ttu-id="26ef5-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="26ef5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26ef5-125">応答</span><span class="sxs-lookup"><span data-stu-id="26ef5-125">Response</span></span>

<span data-ttu-id="26ef5-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="26ef5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26ef5-128">例</span><span class="sxs-lookup"><span data-stu-id="26ef5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26ef5-129">要求</span><span class="sxs-lookup"><span data-stu-id="26ef5-129">Request</span></span>
<span data-ttu-id="26ef5-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26ef5-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="26ef5-131">応答</span><span class="sxs-lookup"><span data-stu-id="26ef5-131">Response</span></span>
<span data-ttu-id="26ef5-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="26ef5-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="26ef5-133">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="26ef5-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="26ef5-134">Visual</span><span class="sxs-lookup"><span data-stu-id="26ef5-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26ef5-135">Java</span><span class="sxs-lookup"><span data-stu-id="26ef5-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
