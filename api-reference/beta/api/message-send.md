---
title: 'メッセージ: send'
description: 下書きフォルダー内のメッセージを送信します。 下書きメッセージは、新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 60c8aaa1e68541074fda4c123146439f55823fb4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333203"
---
# <a name="message-send"></a><span data-ttu-id="29286-104">メッセージ: 送信</span><span class="sxs-lookup"><span data-stu-id="29286-104">message: send</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29286-p102">下書きフォルダー内のメッセージを送信します。新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは転送の下書きが下書きメッセージとなります。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="29286-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="29286-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29286-108">Permissions</span></span>

<span data-ttu-id="29286-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29286-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29286-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29286-111">Permission type</span></span>      | <span data-ttu-id="29286-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29286-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29286-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29286-113">Delegated (work or school account)</span></span> | <span data-ttu-id="29286-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="29286-114">Mail.Send</span></span>    |
|<span data-ttu-id="29286-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29286-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29286-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="29286-116">Mail.Send</span></span>    |
|<span data-ttu-id="29286-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29286-117">Application</span></span> | <span data-ttu-id="29286-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="29286-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="29286-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29286-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="29286-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29286-120">Request headers</span></span>

| <span data-ttu-id="29286-121">名前</span><span class="sxs-lookup"><span data-stu-id="29286-121">Name</span></span>       | <span data-ttu-id="29286-122">型</span><span class="sxs-lookup"><span data-stu-id="29286-122">Type</span></span> | <span data-ttu-id="29286-123">説明</span><span class="sxs-lookup"><span data-stu-id="29286-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="29286-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="29286-124">Authorization</span></span>  | <span data-ttu-id="29286-125">string</span><span class="sxs-lookup"><span data-stu-id="29286-125">string</span></span>  | <span data-ttu-id="29286-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29286-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29286-128">コンテンツの長さ</span><span class="sxs-lookup"><span data-stu-id="29286-128">Content-Length</span></span> | <span data-ttu-id="29286-129">番号</span><span class="sxs-lookup"><span data-stu-id="29286-129">number</span></span> | <span data-ttu-id="29286-130">0. が必要です。</span><span class="sxs-lookup"><span data-stu-id="29286-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29286-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="29286-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="29286-132">応答</span><span class="sxs-lookup"><span data-stu-id="29286-132">Response</span></span>

<span data-ttu-id="29286-p105">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="29286-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29286-135">例</span><span class="sxs-lookup"><span data-stu-id="29286-135">Example</span></span>

<span data-ttu-id="29286-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="29286-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29286-137">要求</span><span class="sxs-lookup"><span data-stu-id="29286-137">Request</span></span>

<span data-ttu-id="29286-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29286-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="29286-139">応答</span><span class="sxs-lookup"><span data-stu-id="29286-139">Response</span></span>

<span data-ttu-id="29286-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="29286-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
