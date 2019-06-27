---
title: 'メッセージ: forward'
description: メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 551a7186c25ae6b0251fa6bcf077ade8358d44fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263736"
---
# <a name="message-forward"></a><span data-ttu-id="f1cc5-104">メッセージ: forward</span><span class="sxs-lookup"><span data-stu-id="f1cc5-104">message: forward</span></span>

<span data-ttu-id="f1cc5-p102">メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1cc5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1cc5-107">Permissions</span></span>
<span data-ttu-id="f1cc5-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1cc5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1cc5-110">Permission type</span></span>      | <span data-ttu-id="f1cc5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1cc5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1cc5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1cc5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1cc5-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f1cc5-113">Mail.Send</span></span>    |
|<span data-ttu-id="f1cc5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1cc5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1cc5-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f1cc5-115">Mail.Send</span></span>    |
|<span data-ttu-id="f1cc5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1cc5-116">Application</span></span> | <span data-ttu-id="f1cc5-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f1cc5-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1cc5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1cc5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="f1cc5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1cc5-119">Request headers</span></span>
| <span data-ttu-id="f1cc5-120">名前</span><span class="sxs-lookup"><span data-stu-id="f1cc5-120">Name</span></span>       | <span data-ttu-id="f1cc5-121">型</span><span class="sxs-lookup"><span data-stu-id="f1cc5-121">Type</span></span> | <span data-ttu-id="f1cc5-122">説明</span><span class="sxs-lookup"><span data-stu-id="f1cc5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1cc5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1cc5-123">Authorization</span></span>  | <span data-ttu-id="f1cc5-124">string</span><span class="sxs-lookup"><span data-stu-id="f1cc5-124">string</span></span>  | <span data-ttu-id="f1cc5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1cc5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1cc5-127">Content-Type</span></span> | <span data-ttu-id="f1cc5-128">string</span><span class="sxs-lookup"><span data-stu-id="f1cc5-128">string</span></span>  | <span data-ttu-id="f1cc5-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1cc5-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1cc5-131">Request body</span></span>
<span data-ttu-id="f1cc5-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f1cc5-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f1cc5-133">Parameter</span></span>    | <span data-ttu-id="f1cc5-134">型</span><span class="sxs-lookup"><span data-stu-id="f1cc5-134">Type</span></span>   |<span data-ttu-id="f1cc5-135">説明</span><span class="sxs-lookup"><span data-stu-id="f1cc5-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1cc5-136">comment</span><span class="sxs-lookup"><span data-stu-id="f1cc5-136">comment</span></span>|<span data-ttu-id="f1cc5-137">String</span><span class="sxs-lookup"><span data-stu-id="f1cc5-137">String</span></span>|<span data-ttu-id="f1cc5-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f1cc5-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="f1cc5-140">toRecipients</span></span>|<span data-ttu-id="f1cc5-141">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="f1cc5-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="f1cc5-142">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="f1cc5-143">応答</span><span class="sxs-lookup"><span data-stu-id="f1cc5-143">Response</span></span>

<span data-ttu-id="f1cc5-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1cc5-146">例</span><span class="sxs-lookup"><span data-stu-id="f1cc5-146">Example</span></span>
<span data-ttu-id="f1cc5-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f1cc5-148">要求</span><span class="sxs-lookup"><span data-stu-id="f1cc5-148">Request</span></span>
<span data-ttu-id="f1cc5-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="f1cc5-150">応答</span><span class="sxs-lookup"><span data-stu-id="f1cc5-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="f1cc5-151">応答</span><span class="sxs-lookup"><span data-stu-id="f1cc5-151">Response</span></span>
<span data-ttu-id="f1cc5-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f1cc5-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1cc5-153">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f1cc5-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1cc5-154">C#</span><span class="sxs-lookup"><span data-stu-id="f1cc5-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1cc5-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1cc5-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_forward-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f1cc5-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="f1cc5-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_forward-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
