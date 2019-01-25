---
title: '投稿: 返信'
description: 'グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。 指定できます。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dfdc25b3e99c26d266631a331d7d58c73042e64b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511136"
---
# <a name="post-reply"></a><span data-ttu-id="9a177-104">投稿: 返信</span><span class="sxs-lookup"><span data-stu-id="9a177-104">post: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a177-p102">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。要求内で親の会話とスレッドの両方を指定するか、または親の会話を使用せずに親スレッドだけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="9a177-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a177-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a177-107">Permissions</span></span>
<span data-ttu-id="9a177-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a177-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a177-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a177-110">Permission type</span></span>      | <span data-ttu-id="9a177-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a177-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a177-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a177-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a177-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a177-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a177-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a177-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a177-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a177-115">Not supported.</span></span>    |
|<span data-ttu-id="9a177-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a177-116">Application</span></span> | <span data-ttu-id="9a177-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a177-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a177-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a177-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="9a177-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a177-119">Request headers</span></span>
| <span data-ttu-id="9a177-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a177-120">Header</span></span>       | <span data-ttu-id="9a177-121">値</span><span class="sxs-lookup"><span data-stu-id="9a177-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a177-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a177-122">Authorization</span></span>  | <span data-ttu-id="9a177-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a177-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a177-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a177-125">Request body</span></span>
<span data-ttu-id="9a177-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a177-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9a177-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a177-127">Parameter</span></span>    | <span data-ttu-id="9a177-128">型</span><span class="sxs-lookup"><span data-stu-id="9a177-128">Type</span></span>   |<span data-ttu-id="9a177-129">説明</span><span class="sxs-lookup"><span data-stu-id="9a177-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a177-130">post</span><span class="sxs-lookup"><span data-stu-id="9a177-130">post</span></span>|[<span data-ttu-id="9a177-131">post</span><span class="sxs-lookup"><span data-stu-id="9a177-131">post</span></span>](../resources/post.md)|<span data-ttu-id="9a177-132">返信中の新規の投稿。</span><span class="sxs-lookup"><span data-stu-id="9a177-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="9a177-133">応答</span><span class="sxs-lookup"><span data-stu-id="9a177-133">Response</span></span>

<span data-ttu-id="9a177-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9a177-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a177-136">例</span><span class="sxs-lookup"><span data-stu-id="9a177-136">Example</span></span>
<span data-ttu-id="9a177-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9a177-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a177-138">要求</span><span class="sxs-lookup"><span data-stu-id="9a177-138">Request</span></span>
<span data-ttu-id="9a177-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a177-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9a177-140">応答</span><span class="sxs-lookup"><span data-stu-id="9a177-140">Response</span></span>
##### <a name="response"></a><span data-ttu-id="9a177-141">応答</span><span class="sxs-lookup"><span data-stu-id="9a177-141">Response</span></span>
<span data-ttu-id="9a177-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9a177-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
