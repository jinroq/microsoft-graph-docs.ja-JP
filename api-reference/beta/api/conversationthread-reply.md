---
title: 'conversationThread: 返信'
description: 'グループの会話のスレッドに返信して、そこに新しい投稿を追加します。 親の会話を指定することができます。 '
author: dkershaw10
ms.openlocfilehash: 9e439901fd2fa9c37ab30c746628e7fcd771edc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314099"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="2d762-104">conversationThread: 返信</span><span class="sxs-lookup"><span data-stu-id="2d762-104">conversationThread: reply</span></span>

> <span data-ttu-id="2d762-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2d762-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d762-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d762-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d762-p103">グループ会話のスレッドに返信して、新しい投稿を追加します。要求内で親の会話を指定したり、親の会話なしにスレッドだけを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="2d762-p103">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d762-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2d762-109">Permissions</span></span>
<span data-ttu-id="2d762-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d762-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d762-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d762-112">Permission type</span></span>      | <span data-ttu-id="2d762-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d762-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d762-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d762-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2d762-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d762-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d762-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d762-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d762-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d762-117">Not supported.</span></span>    |
|<span data-ttu-id="2d762-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d762-118">Application</span></span> | <span data-ttu-id="2d762-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d762-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d762-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d762-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="2d762-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d762-121">Request headers</span></span>
| <span data-ttu-id="2d762-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d762-122">Header</span></span>       | <span data-ttu-id="2d762-123">値</span><span class="sxs-lookup"><span data-stu-id="2d762-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d762-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d762-124">Authorization</span></span>  | <span data-ttu-id="2d762-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2d762-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2d762-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d762-127">Content-Type</span></span>  | <span data-ttu-id="2d762-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2d762-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d762-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d762-130">Request body</span></span>
<span data-ttu-id="2d762-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2d762-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d762-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2d762-132">Parameter</span></span>    | <span data-ttu-id="2d762-133">種類</span><span class="sxs-lookup"><span data-stu-id="2d762-133">Type</span></span>   |<span data-ttu-id="2d762-134">説明</span><span class="sxs-lookup"><span data-stu-id="2d762-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d762-135">post</span><span class="sxs-lookup"><span data-stu-id="2d762-135">post</span></span>|[<span data-ttu-id="2d762-136">post</span><span class="sxs-lookup"><span data-stu-id="2d762-136">post</span></span>](../resources/post.md)|<span data-ttu-id="2d762-137">返信中の新規の投稿。</span><span class="sxs-lookup"><span data-stu-id="2d762-137">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="2d762-138">応答</span><span class="sxs-lookup"><span data-stu-id="2d762-138">Response</span></span>

<span data-ttu-id="2d762-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2d762-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d762-141">例</span><span class="sxs-lookup"><span data-stu-id="2d762-141">Example</span></span>
<span data-ttu-id="2d762-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2d762-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d762-143">要求</span><span class="sxs-lookup"><span data-stu-id="2d762-143">Request</span></span>
<span data-ttu-id="2d762-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d762-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/reply
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

##### <a name="response"></a><span data-ttu-id="2d762-145">応答</span><span class="sxs-lookup"><span data-stu-id="2d762-145">Response</span></span>
<span data-ttu-id="2d762-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2d762-146">Here is an example of the response.</span></span>
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
