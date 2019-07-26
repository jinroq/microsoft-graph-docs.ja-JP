---
title: 'メッセージ: send'
description: 下書きフォルダー内のメッセージを送信します。 下書きメッセージは、新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2d8b3dd07fc6db4bdd49c122ab9bcf844bd57d19
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884700"
---
# <a name="message-send"></a><span data-ttu-id="ea753-104">メッセージ: 送信</span><span class="sxs-lookup"><span data-stu-id="ea753-104">message: send</span></span>

<span data-ttu-id="ea753-p102">下書きフォルダー内のメッセージを送信します。新しい下書きメッセージ、返信の下書き、全員へ返信の下書き、あるいは転送の下書きが下書きメッセージとなります。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="ea753-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea753-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea753-108">Permissions</span></span>

<span data-ttu-id="ea753-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea753-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea753-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea753-111">Permission type</span></span>      | <span data-ttu-id="ea753-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea753-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea753-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea753-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ea753-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ea753-114">Mail.Send</span></span>    |
|<span data-ttu-id="ea753-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea753-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea753-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ea753-116">Mail.Send</span></span>    |
|<span data-ttu-id="ea753-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea753-117">Application</span></span> | <span data-ttu-id="ea753-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ea753-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea753-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea753-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="ea753-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea753-120">Request headers</span></span>

| <span data-ttu-id="ea753-121">名前</span><span class="sxs-lookup"><span data-stu-id="ea753-121">Name</span></span>       | <span data-ttu-id="ea753-122">型</span><span class="sxs-lookup"><span data-stu-id="ea753-122">Type</span></span> | <span data-ttu-id="ea753-123">説明</span><span class="sxs-lookup"><span data-stu-id="ea753-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ea753-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea753-124">Authorization</span></span>  | <span data-ttu-id="ea753-125">string</span><span class="sxs-lookup"><span data-stu-id="ea753-125">string</span></span>  | <span data-ttu-id="ea753-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea753-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea753-128">コンテンツの長さ</span><span class="sxs-lookup"><span data-stu-id="ea753-128">Content-Length</span></span> | <span data-ttu-id="ea753-129">番号</span><span class="sxs-lookup"><span data-stu-id="ea753-129">number</span></span> | <span data-ttu-id="ea753-130">0. が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea753-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea753-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea753-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ea753-132">応答</span><span class="sxs-lookup"><span data-stu-id="ea753-132">Response</span></span>

<span data-ttu-id="ea753-p105">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ea753-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea753-135">例</span><span class="sxs-lookup"><span data-stu-id="ea753-135">Example</span></span>

<span data-ttu-id="ea753-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ea753-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ea753-137">要求</span><span class="sxs-lookup"><span data-stu-id="ea753-137">Request</span></span>

<span data-ttu-id="ea753-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea753-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ea753-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea753-139">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ea753-140">C#</span><span class="sxs-lookup"><span data-stu-id="ea753-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ea753-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="ea753-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ea753-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea753-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ea753-143">Java</span><span class="sxs-lookup"><span data-stu-id="ea753-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ea753-144">応答</span><span class="sxs-lookup"><span data-stu-id="ea753-144">Response</span></span>

<span data-ttu-id="ea753-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ea753-145">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
