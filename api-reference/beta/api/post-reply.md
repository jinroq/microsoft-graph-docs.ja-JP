---
title: '投稿: 返信'
description: 'グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。 指定できます。 '
author: dkershaw10
ms.openlocfilehash: 33cd99fd24dc5acfca4b96f232f748a0377d1564
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324228"
---
# <a name="post-reply"></a><span data-ttu-id="851df-104">投稿: 返信</span><span class="sxs-lookup"><span data-stu-id="851df-104">post: reply</span></span>

> <span data-ttu-id="851df-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="851df-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="851df-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="851df-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="851df-p103">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。要求内で親の会話とスレッドの両方を指定するか、または親の会話を使用せずに親スレッドだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="851df-p103">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="851df-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="851df-109">Permissions</span></span>
<span data-ttu-id="851df-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="851df-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="851df-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="851df-112">Permission type</span></span>      | <span data-ttu-id="851df-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="851df-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="851df-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="851df-114">Delegated (work or school account)</span></span> | <span data-ttu-id="851df-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="851df-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="851df-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="851df-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="851df-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="851df-117">Not supported.</span></span>    |
|<span data-ttu-id="851df-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="851df-118">Application</span></span> | <span data-ttu-id="851df-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="851df-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="851df-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="851df-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="851df-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="851df-121">Request headers</span></span>
| <span data-ttu-id="851df-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="851df-122">Header</span></span>       | <span data-ttu-id="851df-123">値</span><span class="sxs-lookup"><span data-stu-id="851df-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="851df-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="851df-124">Authorization</span></span>  | <span data-ttu-id="851df-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="851df-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="851df-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="851df-127">Request body</span></span>
<span data-ttu-id="851df-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="851df-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="851df-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="851df-129">Parameter</span></span>    | <span data-ttu-id="851df-130">種類</span><span class="sxs-lookup"><span data-stu-id="851df-130">Type</span></span>   |<span data-ttu-id="851df-131">説明</span><span class="sxs-lookup"><span data-stu-id="851df-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="851df-132">post</span><span class="sxs-lookup"><span data-stu-id="851df-132">post</span></span>|[<span data-ttu-id="851df-133">post</span><span class="sxs-lookup"><span data-stu-id="851df-133">post</span></span>](../resources/post.md)|<span data-ttu-id="851df-134">返信中の新規の投稿。</span><span class="sxs-lookup"><span data-stu-id="851df-134">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="851df-135">応答</span><span class="sxs-lookup"><span data-stu-id="851df-135">Response</span></span>

<span data-ttu-id="851df-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="851df-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="851df-138">例</span><span class="sxs-lookup"><span data-stu-id="851df-138">Example</span></span>
<span data-ttu-id="851df-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="851df-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="851df-140">要求</span><span class="sxs-lookup"><span data-stu-id="851df-140">Request</span></span>
<span data-ttu-id="851df-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="851df-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "2016-10-19T10:37:00Z",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "2016-10-19T10:37:00Z",
    "lastModifiedDateTime": "2016-10-19T10:37:00Z",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "2016-10-19T10:37:00Z",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="851df-142">応答</span><span class="sxs-lookup"><span data-stu-id="851df-142">Response</span></span>
##### <a name="response"></a><span data-ttu-id="851df-143">応答</span><span class="sxs-lookup"><span data-stu-id="851df-143">Response</span></span>
<span data-ttu-id="851df-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="851df-144">Here is an example of the response.</span></span>
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
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
