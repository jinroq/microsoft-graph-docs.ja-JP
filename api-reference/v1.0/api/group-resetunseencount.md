---
title: 'グループ: resetUnseenCount'
description: 現在のユーザーが最後の訪問以降見ていない、すべての投稿の unseenCount をリセットします。Office 365 のグループのみをサポートします。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 035d53537587fde0c6ab0b33fd08fbe7987e1fbd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613937"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="a5398-104">グループ: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="a5398-104">group: resetUnseenCount</span></span>
<span data-ttu-id="a5398-p102">現在のユーザーが最後の訪問以降見ていない、すべての投稿の unseenCount をリセットします。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="a5398-p102">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5398-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5398-107">Permissions</span></span>
<span data-ttu-id="a5398-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5398-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5398-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5398-110">Permission type</span></span>      | <span data-ttu-id="a5398-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5398-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5398-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5398-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5398-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5398-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5398-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5398-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5398-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5398-115">Not supported.</span></span>    |
|<span data-ttu-id="a5398-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5398-116">Application</span></span> | <span data-ttu-id="a5398-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5398-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5398-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5398-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="a5398-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5398-119">Request headers</span></span>
| <span data-ttu-id="a5398-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5398-120">Header</span></span>       | <span data-ttu-id="a5398-121">値</span><span class="sxs-lookup"><span data-stu-id="a5398-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5398-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5398-122">Authorization</span></span>  | <span data-ttu-id="a5398-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a5398-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5398-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="a5398-125">Prefer</span></span> | <span data-ttu-id="a5398-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="a5398-126">return=minimal.</span></span> <span data-ttu-id="a5398-127">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="a5398-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="a5398-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a5398-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="a5398-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5398-129">Request body</span></span>
<span data-ttu-id="a5398-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a5398-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5398-131">応答</span><span class="sxs-lookup"><span data-stu-id="a5398-131">Response</span></span>
<span data-ttu-id="a5398-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a5398-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5398-134">例</span><span class="sxs-lookup"><span data-stu-id="a5398-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a5398-135">要求</span><span class="sxs-lookup"><span data-stu-id="a5398-135">Request</span></span>
<span data-ttu-id="a5398-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5398-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="a5398-137">応答</span><span class="sxs-lookup"><span data-stu-id="a5398-137">Response</span></span>
<span data-ttu-id="a5398-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5398-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5398-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="a5398-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5398-140">Visual</span><span class="sxs-lookup"><span data-stu-id="a5398-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_resetunseencount-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5398-141">Java</span><span class="sxs-lookup"><span data-stu-id="a5398-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_resetunseencount-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-resetunseencount.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-resetunseencount.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
