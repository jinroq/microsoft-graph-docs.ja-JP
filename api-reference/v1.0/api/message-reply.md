---
title: 'メッセージ: reply'
description: メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7321b424046a327f5d0e87c477aad8ab14f082e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856287"
---
# <a name="message-reply"></a><span data-ttu-id="c1db3-104">メッセージ: reply</span><span class="sxs-lookup"><span data-stu-id="c1db3-104">message: reply</span></span>

<span data-ttu-id="c1db3-p102">メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="c1db3-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1db3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c1db3-107">Permissions</span></span>
<span data-ttu-id="c1db3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1db3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1db3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1db3-110">Permission type</span></span>      | <span data-ttu-id="c1db3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1db3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1db3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1db3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1db3-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c1db3-113">Mail.Send</span></span>    |
|<span data-ttu-id="c1db3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1db3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1db3-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c1db3-115">Mail.Send</span></span>    |
|<span data-ttu-id="c1db3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1db3-116">Application</span></span> | <span data-ttu-id="c1db3-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c1db3-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1db3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1db3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="c1db3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1db3-119">Request headers</span></span>
| <span data-ttu-id="c1db3-120">名前</span><span class="sxs-lookup"><span data-stu-id="c1db3-120">Name</span></span>       | <span data-ttu-id="c1db3-121">型</span><span class="sxs-lookup"><span data-stu-id="c1db3-121">Type</span></span> | <span data-ttu-id="c1db3-122">説明</span><span class="sxs-lookup"><span data-stu-id="c1db3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c1db3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1db3-123">Authorization</span></span>  | <span data-ttu-id="c1db3-124">string</span><span class="sxs-lookup"><span data-stu-id="c1db3-124">string</span></span>  | <span data-ttu-id="c1db3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c1db3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1db3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1db3-127">Content-Type</span></span> | <span data-ttu-id="c1db3-128">string</span><span class="sxs-lookup"><span data-stu-id="c1db3-128">string</span></span>  | <span data-ttu-id="c1db3-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="c1db3-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1db3-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1db3-131">Request body</span></span>
<span data-ttu-id="c1db3-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c1db3-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1db3-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c1db3-133">Parameter</span></span>    | <span data-ttu-id="c1db3-134">型</span><span class="sxs-lookup"><span data-stu-id="c1db3-134">Type</span></span>   |<span data-ttu-id="c1db3-135">説明</span><span class="sxs-lookup"><span data-stu-id="c1db3-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1db3-136">comment</span><span class="sxs-lookup"><span data-stu-id="c1db3-136">comment</span></span>|<span data-ttu-id="c1db3-137">String</span><span class="sxs-lookup"><span data-stu-id="c1db3-137">String</span></span>|<span data-ttu-id="c1db3-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c1db3-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="c1db3-140">応答</span><span class="sxs-lookup"><span data-stu-id="c1db3-140">Response</span></span>

<span data-ttu-id="c1db3-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c1db3-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1db3-143">例</span><span class="sxs-lookup"><span data-stu-id="c1db3-143">Example</span></span>
<span data-ttu-id="c1db3-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c1db3-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1db3-145">要求</span><span class="sxs-lookup"><span data-stu-id="c1db3-145">Request</span></span>
<span data-ttu-id="c1db3-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c1db3-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1db3-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c1db3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1db3-148">C#</span><span class="sxs-lookup"><span data-stu-id="c1db3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1db3-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1db3-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1db3-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="c1db3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c1db3-151">Java</span><span class="sxs-lookup"><span data-stu-id="c1db3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c1db3-152">応答</span><span class="sxs-lookup"><span data-stu-id="c1db3-152">Response</span></span>
##### <a name="response"></a><span data-ttu-id="c1db3-153">応答</span><span class="sxs-lookup"><span data-stu-id="c1db3-153">Response</span></span>
<span data-ttu-id="c1db3-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c1db3-154">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
