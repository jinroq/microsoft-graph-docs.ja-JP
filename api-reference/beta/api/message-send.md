---
title: 'メッセージ: send'
description: 下書きフォルダーにメッセージを送信します。 下書きメッセージは、新しいメッセージの下書き、ドラフトの返信、全員に返信、下書き、または
localization_priority: Normal
ms.openlocfilehash: 6ccef4d1a58faea7678acefee5d175403a8827b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806644"
---
# <a name="message-send"></a><span data-ttu-id="9c430-104">メッセージ: send</span><span class="sxs-lookup"><span data-stu-id="9c430-104">message: send</span></span>

> <span data-ttu-id="9c430-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c430-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c430-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c430-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c430-p103">下書きフォルダー内のメッセージを送信します。新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは転送の下書きが下書きメッセージとなります。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="9c430-p103">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c430-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9c430-110">Permissions</span></span>

<span data-ttu-id="9c430-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c430-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c430-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9c430-113">Permission type</span></span>      | <span data-ttu-id="9c430-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9c430-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c430-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9c430-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9c430-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c430-116">Mail.Send</span></span>    |
|<span data-ttu-id="9c430-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9c430-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c430-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c430-118">Mail.Send</span></span>    |
|<span data-ttu-id="9c430-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9c430-119">Application</span></span> | <span data-ttu-id="9c430-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c430-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c430-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9c430-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="9c430-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c430-122">Request headers</span></span>

| <span data-ttu-id="9c430-123">名前</span><span class="sxs-lookup"><span data-stu-id="9c430-123">Name</span></span>       | <span data-ttu-id="9c430-124">種類</span><span class="sxs-lookup"><span data-stu-id="9c430-124">Type</span></span> | <span data-ttu-id="9c430-125">説明</span><span class="sxs-lookup"><span data-stu-id="9c430-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c430-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c430-126">Authorization</span></span>  | <span data-ttu-id="9c430-127">string</span><span class="sxs-lookup"><span data-stu-id="9c430-127">string</span></span>  | <span data-ttu-id="9c430-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9c430-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c430-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="9c430-130">Content-Length</span></span> | <span data-ttu-id="9c430-131">number</span><span class="sxs-lookup"><span data-stu-id="9c430-131">number</span></span> | <span data-ttu-id="9c430-132">0 が必要です。</span><span class="sxs-lookup"><span data-stu-id="9c430-132">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c430-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="9c430-133">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9c430-134">応答</span><span class="sxs-lookup"><span data-stu-id="9c430-134">Response</span></span>

<span data-ttu-id="9c430-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9c430-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c430-137">例</span><span class="sxs-lookup"><span data-stu-id="9c430-137">Example</span></span>

<span data-ttu-id="9c430-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9c430-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9c430-139">要求</span><span class="sxs-lookup"><span data-stu-id="9c430-139">Request</span></span>

<span data-ttu-id="9c430-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9c430-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="9c430-141">応答</span><span class="sxs-lookup"><span data-stu-id="9c430-141">Response</span></span>

<span data-ttu-id="9c430-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9c430-142">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
