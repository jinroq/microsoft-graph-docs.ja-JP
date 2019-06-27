---
title: 'メッセージ: reply'
description: メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d65dc2c3dc036322d130cdd81979fab11d3b7842
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274593"
---
# <a name="message-reply"></a><span data-ttu-id="e99a0-104">メッセージ: reply</span><span class="sxs-lookup"><span data-stu-id="e99a0-104">message: reply</span></span>

<span data-ttu-id="e99a0-p102">メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="e99a0-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="e99a0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e99a0-107">Permissions</span></span>
<span data-ttu-id="e99a0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e99a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e99a0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e99a0-110">Permission type</span></span>      | <span data-ttu-id="e99a0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e99a0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e99a0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e99a0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e99a0-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e99a0-113">Mail.Send</span></span>    |
|<span data-ttu-id="e99a0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e99a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e99a0-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e99a0-115">Mail.Send</span></span>    |
|<span data-ttu-id="e99a0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e99a0-116">Application</span></span> | <span data-ttu-id="e99a0-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e99a0-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e99a0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e99a0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="e99a0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e99a0-119">Request headers</span></span>
| <span data-ttu-id="e99a0-120">名前</span><span class="sxs-lookup"><span data-stu-id="e99a0-120">Name</span></span>       | <span data-ttu-id="e99a0-121">型</span><span class="sxs-lookup"><span data-stu-id="e99a0-121">Type</span></span> | <span data-ttu-id="e99a0-122">説明</span><span class="sxs-lookup"><span data-stu-id="e99a0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e99a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e99a0-123">Authorization</span></span>  | <span data-ttu-id="e99a0-124">string</span><span class="sxs-lookup"><span data-stu-id="e99a0-124">string</span></span>  | <span data-ttu-id="e99a0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e99a0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e99a0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e99a0-127">Content-Type</span></span> | <span data-ttu-id="e99a0-128">string</span><span class="sxs-lookup"><span data-stu-id="e99a0-128">string</span></span>  | <span data-ttu-id="e99a0-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="e99a0-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e99a0-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="e99a0-131">Request body</span></span>
<span data-ttu-id="e99a0-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e99a0-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e99a0-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e99a0-133">Parameter</span></span>    | <span data-ttu-id="e99a0-134">型</span><span class="sxs-lookup"><span data-stu-id="e99a0-134">Type</span></span>   |<span data-ttu-id="e99a0-135">説明</span><span class="sxs-lookup"><span data-stu-id="e99a0-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e99a0-136">comment</span><span class="sxs-lookup"><span data-stu-id="e99a0-136">comment</span></span>|<span data-ttu-id="e99a0-137">String</span><span class="sxs-lookup"><span data-stu-id="e99a0-137">String</span></span>|<span data-ttu-id="e99a0-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e99a0-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="e99a0-140">応答</span><span class="sxs-lookup"><span data-stu-id="e99a0-140">Response</span></span>

<span data-ttu-id="e99a0-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e99a0-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e99a0-143">例</span><span class="sxs-lookup"><span data-stu-id="e99a0-143">Example</span></span>
<span data-ttu-id="e99a0-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e99a0-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e99a0-145">要求</span><span class="sxs-lookup"><span data-stu-id="e99a0-145">Request</span></span>
<span data-ttu-id="e99a0-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e99a0-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e99a0-147">応答</span><span class="sxs-lookup"><span data-stu-id="e99a0-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="e99a0-148">応答</span><span class="sxs-lookup"><span data-stu-id="e99a0-148">Response</span></span>
<span data-ttu-id="e99a0-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e99a0-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e99a0-150">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e99a0-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e99a0-151">C#</span><span class="sxs-lookup"><span data-stu-id="e99a0-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e99a0-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="e99a0-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_reply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e99a0-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="e99a0-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_reply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
