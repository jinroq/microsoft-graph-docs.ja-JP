---
title: 'メッセージ: forward'
description: メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 01c849e9d11e9ce11daf9ff25248cd9279209766
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612411"
---
# <a name="message-forward"></a><span data-ttu-id="f12f1-104">メッセージ: forward</span><span class="sxs-lookup"><span data-stu-id="f12f1-104">message: forward</span></span>

<span data-ttu-id="f12f1-p102">メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="f12f1-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="f12f1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f12f1-107">Permissions</span></span>
<span data-ttu-id="f12f1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f12f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f12f1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f12f1-110">Permission type</span></span>      | <span data-ttu-id="f12f1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f12f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f12f1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f12f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f12f1-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f12f1-113">Mail.Send</span></span>    |
|<span data-ttu-id="f12f1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f12f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f12f1-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f12f1-115">Mail.Send</span></span>    |
|<span data-ttu-id="f12f1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f12f1-116">Application</span></span> | <span data-ttu-id="f12f1-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f12f1-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f12f1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f12f1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="f12f1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f12f1-119">Request headers</span></span>
| <span data-ttu-id="f12f1-120">名前</span><span class="sxs-lookup"><span data-stu-id="f12f1-120">Name</span></span>       | <span data-ttu-id="f12f1-121">型</span><span class="sxs-lookup"><span data-stu-id="f12f1-121">Type</span></span> | <span data-ttu-id="f12f1-122">説明</span><span class="sxs-lookup"><span data-stu-id="f12f1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f12f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f12f1-123">Authorization</span></span>  | <span data-ttu-id="f12f1-124">string</span><span class="sxs-lookup"><span data-stu-id="f12f1-124">string</span></span>  | <span data-ttu-id="f12f1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f12f1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f12f1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f12f1-127">Content-Type</span></span> | <span data-ttu-id="f12f1-128">string</span><span class="sxs-lookup"><span data-stu-id="f12f1-128">string</span></span>  | <span data-ttu-id="f12f1-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="f12f1-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f12f1-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="f12f1-131">Request body</span></span>
<span data-ttu-id="f12f1-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f12f1-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f12f1-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f12f1-133">Parameter</span></span>    | <span data-ttu-id="f12f1-134">型</span><span class="sxs-lookup"><span data-stu-id="f12f1-134">Type</span></span>   |<span data-ttu-id="f12f1-135">説明</span><span class="sxs-lookup"><span data-stu-id="f12f1-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f12f1-136">comment</span><span class="sxs-lookup"><span data-stu-id="f12f1-136">comment</span></span>|<span data-ttu-id="f12f1-137">String</span><span class="sxs-lookup"><span data-stu-id="f12f1-137">String</span></span>|<span data-ttu-id="f12f1-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f12f1-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f12f1-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="f12f1-140">toRecipients</span></span>|<span data-ttu-id="f12f1-141">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="f12f1-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="f12f1-142">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f12f1-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="f12f1-143">応答</span><span class="sxs-lookup"><span data-stu-id="f12f1-143">Response</span></span>

<span data-ttu-id="f12f1-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f12f1-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f12f1-146">例</span><span class="sxs-lookup"><span data-stu-id="f12f1-146">Example</span></span>
<span data-ttu-id="f12f1-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f12f1-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f12f1-148">要求</span><span class="sxs-lookup"><span data-stu-id="f12f1-148">Request</span></span>
<span data-ttu-id="f12f1-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f12f1-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f12f1-150">応答</span><span class="sxs-lookup"><span data-stu-id="f12f1-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="f12f1-151">応答</span><span class="sxs-lookup"><span data-stu-id="f12f1-151">Response</span></span>
<span data-ttu-id="f12f1-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f12f1-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f12f1-153">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="f12f1-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f12f1-154">Visual</span><span class="sxs-lookup"><span data-stu-id="f12f1-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f12f1-155">Java</span><span class="sxs-lookup"><span data-stu-id="f12f1-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_forward-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
