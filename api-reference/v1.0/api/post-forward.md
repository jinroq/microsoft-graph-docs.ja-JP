---
title: '投稿: 転送'
description: '受信者に投稿を転送します。 要求に親スレッドとスレッドの両方を指定することができます。 '
localization_priority: Normal
ms.openlocfilehash: b670338061d70b4ee8663d443d1bb5706f9e9157
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837325"
---
# <a name="post-forward"></a><span data-ttu-id="e1d99-104">投稿: 転送</span><span class="sxs-lookup"><span data-stu-id="e1d99-104">post: forward</span></span>

<span data-ttu-id="e1d99-p102">受信者に投稿を転送します。要求内で親の会話とスレッドの両方を指定するか、または親の会話を使用せずに親スレッドだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="e1d99-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e1d99-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1d99-107">Permissions</span></span>
<span data-ttu-id="e1d99-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1d99-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1d99-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1d99-110">Permission type</span></span>      | <span data-ttu-id="e1d99-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1d99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1d99-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1d99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e1d99-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1d99-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1d99-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1d99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1d99-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1d99-115">Not supported.</span></span>    |
|<span data-ttu-id="e1d99-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1d99-116">Application</span></span> | <span data-ttu-id="e1d99-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1d99-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1d99-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1d99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="e1d99-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1d99-119">Request headers</span></span>
| <span data-ttu-id="e1d99-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1d99-120">Header</span></span>       | <span data-ttu-id="e1d99-121">値</span><span class="sxs-lookup"><span data-stu-id="e1d99-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1d99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1d99-122">Authorization</span></span>  | <span data-ttu-id="e1d99-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1d99-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1d99-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1d99-125">Request body</span></span>
<span data-ttu-id="e1d99-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e1d99-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e1d99-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e1d99-127">Parameter</span></span>    | <span data-ttu-id="e1d99-128">Type</span><span class="sxs-lookup"><span data-stu-id="e1d99-128">Type</span></span>   |<span data-ttu-id="e1d99-129">説明</span><span class="sxs-lookup"><span data-stu-id="e1d99-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1d99-130">comment</span><span class="sxs-lookup"><span data-stu-id="e1d99-130">comment</span></span>|<span data-ttu-id="e1d99-131">String</span><span class="sxs-lookup"><span data-stu-id="e1d99-131">String</span></span>|<span data-ttu-id="e1d99-132">投稿と共に転送されるオプションのコメント。</span><span class="sxs-lookup"><span data-stu-id="e1d99-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="e1d99-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="e1d99-133">toRecipients</span></span>|<span data-ttu-id="e1d99-134">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="e1d99-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="e1d99-135">スレッドの転送先となる受信者。</span><span class="sxs-lookup"><span data-stu-id="e1d99-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="e1d99-136">応答</span><span class="sxs-lookup"><span data-stu-id="e1d99-136">Response</span></span>

<span data-ttu-id="e1d99-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e1d99-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1d99-139">例</span><span class="sxs-lookup"><span data-stu-id="e1d99-139">Example</span></span>
<span data-ttu-id="e1d99-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e1d99-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e1d99-141">要求</span><span class="sxs-lookup"><span data-stu-id="e1d99-141">Request</span></span>
<span data-ttu-id="e1d99-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1d99-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="e1d99-143">応答</span><span class="sxs-lookup"><span data-stu-id="e1d99-143">Response</span></span>
<span data-ttu-id="e1d99-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e1d99-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
