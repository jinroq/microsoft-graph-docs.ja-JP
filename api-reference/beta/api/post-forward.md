---
title: '投稿: 転送'
description: '受信者に投稿を転送します。 要求には、親の会話とスレッドの両方を指定できます。 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: cf8d8c7759eec6f2429d16b791480ebcf531145c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264254"
---
# <a name="post-forward"></a><span data-ttu-id="87c18-104">投稿: 転送</span><span class="sxs-lookup"><span data-stu-id="87c18-104">post: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87c18-p102">受信者に投稿を転送します。要求内で親の会話とスレッドの両方を指定するか、または親の会話を使用せずに親スレッドだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="87c18-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="87c18-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87c18-107">Permissions</span></span>
<span data-ttu-id="87c18-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87c18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87c18-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87c18-110">Permission type</span></span>      | <span data-ttu-id="87c18-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87c18-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c18-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87c18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87c18-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87c18-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="87c18-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87c18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c18-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87c18-115">Not supported.</span></span>    |
|<span data-ttu-id="87c18-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87c18-116">Application</span></span> | <span data-ttu-id="87c18-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87c18-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87c18-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87c18-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="87c18-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87c18-119">Request headers</span></span>
| <span data-ttu-id="87c18-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87c18-120">Header</span></span>       | <span data-ttu-id="87c18-121">値</span><span class="sxs-lookup"><span data-stu-id="87c18-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87c18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87c18-122">Authorization</span></span>  | <span data-ttu-id="87c18-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="87c18-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87c18-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="87c18-125">Request body</span></span>
<span data-ttu-id="87c18-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="87c18-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87c18-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="87c18-127">Parameter</span></span>    | <span data-ttu-id="87c18-128">型</span><span class="sxs-lookup"><span data-stu-id="87c18-128">Type</span></span>   |<span data-ttu-id="87c18-129">説明</span><span class="sxs-lookup"><span data-stu-id="87c18-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87c18-130">comment</span><span class="sxs-lookup"><span data-stu-id="87c18-130">comment</span></span>|<span data-ttu-id="87c18-131">String</span><span class="sxs-lookup"><span data-stu-id="87c18-131">String</span></span>|<span data-ttu-id="87c18-132">投稿と共に転送されるオプションのコメント。</span><span class="sxs-lookup"><span data-stu-id="87c18-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="87c18-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="87c18-133">toRecipients</span></span>|<span data-ttu-id="87c18-134">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="87c18-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="87c18-135">スレッドの転送先となる受信者。</span><span class="sxs-lookup"><span data-stu-id="87c18-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="87c18-136">応答</span><span class="sxs-lookup"><span data-stu-id="87c18-136">Response</span></span>

<span data-ttu-id="87c18-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="87c18-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87c18-139">例</span><span class="sxs-lookup"><span data-stu-id="87c18-139">Example</span></span>
<span data-ttu-id="87c18-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="87c18-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87c18-141">要求</span><span class="sxs-lookup"><span data-stu-id="87c18-141">Request</span></span>
<span data-ttu-id="87c18-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87c18-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="87c18-143">応答</span><span class="sxs-lookup"><span data-stu-id="87c18-143">Response</span></span>
<span data-ttu-id="87c18-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="87c18-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="87c18-145">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="87c18-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="87c18-146">C#</span><span class="sxs-lookup"><span data-stu-id="87c18-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87c18-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="87c18-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_forward-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="87c18-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="87c18-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/post_forward-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
