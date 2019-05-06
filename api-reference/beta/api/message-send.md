---
title: 'メッセージ: send'
description: 下書きフォルダー内のメッセージを送信します。 下書きメッセージは、新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c4a4010a69f3c6323ab624d2b1fa1f16075a519b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597766"
---
# <a name="message-send"></a><span data-ttu-id="b3c1f-104">メッセージ: 送信</span><span class="sxs-lookup"><span data-stu-id="b3c1f-104">message: send</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3c1f-p102">下書きフォルダー内のメッセージを送信します。新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは転送の下書きが下書きメッセージとなります。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="b3c1f-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3c1f-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3c1f-108">Permissions</span></span>

<span data-ttu-id="b3c1f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3c1f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3c1f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3c1f-111">Permission type</span></span>      | <span data-ttu-id="b3c1f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3c1f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3c1f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3c1f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b3c1f-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b3c1f-114">Mail.Send</span></span>    |
|<span data-ttu-id="b3c1f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3c1f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3c1f-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b3c1f-116">Mail.Send</span></span>    |
|<span data-ttu-id="b3c1f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3c1f-117">Application</span></span> | <span data-ttu-id="b3c1f-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b3c1f-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3c1f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3c1f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="b3c1f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3c1f-120">Request headers</span></span>

| <span data-ttu-id="b3c1f-121">名前</span><span class="sxs-lookup"><span data-stu-id="b3c1f-121">Name</span></span>       | <span data-ttu-id="b3c1f-122">型</span><span class="sxs-lookup"><span data-stu-id="b3c1f-122">Type</span></span> | <span data-ttu-id="b3c1f-123">説明</span><span class="sxs-lookup"><span data-stu-id="b3c1f-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3c1f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3c1f-124">Authorization</span></span>  | <span data-ttu-id="b3c1f-125">string</span><span class="sxs-lookup"><span data-stu-id="b3c1f-125">string</span></span>  | <span data-ttu-id="b3c1f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b3c1f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3c1f-128">コンテンツの長さ</span><span class="sxs-lookup"><span data-stu-id="b3c1f-128">Content-Length</span></span> | <span data-ttu-id="b3c1f-129">番号</span><span class="sxs-lookup"><span data-stu-id="b3c1f-129">number</span></span> | <span data-ttu-id="b3c1f-130">0. が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3c1f-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3c1f-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3c1f-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b3c1f-132">応答</span><span class="sxs-lookup"><span data-stu-id="b3c1f-132">Response</span></span>

<span data-ttu-id="b3c1f-p105">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b3c1f-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3c1f-135">例</span><span class="sxs-lookup"><span data-stu-id="b3c1f-135">Example</span></span>

<span data-ttu-id="b3c1f-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b3c1f-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b3c1f-137">要求</span><span class="sxs-lookup"><span data-stu-id="b3c1f-137">Request</span></span>

<span data-ttu-id="b3c1f-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3c1f-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="b3c1f-139">応答</span><span class="sxs-lookup"><span data-stu-id="b3c1f-139">Response</span></span>

<span data-ttu-id="b3c1f-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b3c1f-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b3c1f-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="b3c1f-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b3c1f-142">Visual</span><span class="sxs-lookup"><span data-stu-id="b3c1f-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_send-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3c1f-143">Java</span><span class="sxs-lookup"><span data-stu-id="b3c1f-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_send-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-send.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-send.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
