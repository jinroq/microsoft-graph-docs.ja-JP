---
title: 'conversationThread: 返信'
description: 'グループの会話のスレッドに返信して、そこに新しい投稿を追加します。 親の会話を指定することができます。 '
ms.openlocfilehash: ca252cb578c0b04cddead455ca046d13180626e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022781"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="91d2f-104">conversationThread: 返信</span><span class="sxs-lookup"><span data-stu-id="91d2f-104">conversationThread: reply</span></span>

<span data-ttu-id="91d2f-p102">グループ会話のスレッドに返信して、新しい投稿を追加します。要求内で親の会話を指定したり、親の会話なしにスレッドだけを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="91d2f-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="91d2f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91d2f-107">Permissions</span></span>
<span data-ttu-id="91d2f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91d2f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91d2f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91d2f-110">Permission type</span></span>      | <span data-ttu-id="91d2f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91d2f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91d2f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91d2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91d2f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91d2f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="91d2f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91d2f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91d2f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91d2f-115">Not supported.</span></span>    |
|<span data-ttu-id="91d2f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91d2f-116">Application</span></span> | <span data-ttu-id="91d2f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91d2f-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91d2f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91d2f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="91d2f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91d2f-119">Request headers</span></span>
| <span data-ttu-id="91d2f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91d2f-120">Header</span></span>       | <span data-ttu-id="91d2f-121">値</span><span class="sxs-lookup"><span data-stu-id="91d2f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91d2f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91d2f-122">Authorization</span></span>  | <span data-ttu-id="91d2f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="91d2f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91d2f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91d2f-125">Content-Type</span></span>  | <span data-ttu-id="91d2f-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="91d2f-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91d2f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="91d2f-128">Request body</span></span>
<span data-ttu-id="91d2f-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="91d2f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="91d2f-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="91d2f-130">Parameter</span></span>    | <span data-ttu-id="91d2f-131">型</span><span class="sxs-lookup"><span data-stu-id="91d2f-131">Type</span></span>   |<span data-ttu-id="91d2f-132">説明</span><span class="sxs-lookup"><span data-stu-id="91d2f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91d2f-133">post</span><span class="sxs-lookup"><span data-stu-id="91d2f-133">post</span></span>|[<span data-ttu-id="91d2f-134">post</span><span class="sxs-lookup"><span data-stu-id="91d2f-134">post</span></span>](../resources/post.md)|<span data-ttu-id="91d2f-135">返信中の新規の投稿。</span><span class="sxs-lookup"><span data-stu-id="91d2f-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="91d2f-136">応答</span><span class="sxs-lookup"><span data-stu-id="91d2f-136">Response</span></span>

<span data-ttu-id="91d2f-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="91d2f-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91d2f-139">例</span><span class="sxs-lookup"><span data-stu-id="91d2f-139">Example</span></span>
<span data-ttu-id="91d2f-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="91d2f-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91d2f-141">要求</span><span class="sxs-lookup"><span data-stu-id="91d2f-141">Request</span></span>
<span data-ttu-id="91d2f-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91d2f-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="91d2f-143">応答</span><span class="sxs-lookup"><span data-stu-id="91d2f-143">Response</span></span>
<span data-ttu-id="91d2f-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="91d2f-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->