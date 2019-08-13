---
title: 'メッセージ: forward'
description: メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f3d568d4e519ab17d39bd01eabe28830ea29d17c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374765"
---
# <a name="message-forward"></a><span data-ttu-id="c212d-104">メッセージ: forward</span><span class="sxs-lookup"><span data-stu-id="c212d-104">message: forward</span></span>

<span data-ttu-id="c212d-p102">メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="c212d-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c212d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c212d-107">Permissions</span></span>
<span data-ttu-id="c212d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c212d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c212d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c212d-110">Permission type</span></span>      | <span data-ttu-id="c212d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c212d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c212d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c212d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c212d-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c212d-113">Mail.Send</span></span>    |
|<span data-ttu-id="c212d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c212d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c212d-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c212d-115">Mail.Send</span></span>    |
|<span data-ttu-id="c212d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c212d-116">Application</span></span> | <span data-ttu-id="c212d-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c212d-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c212d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c212d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="c212d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c212d-119">Request headers</span></span>
| <span data-ttu-id="c212d-120">名前</span><span class="sxs-lookup"><span data-stu-id="c212d-120">Name</span></span>       | <span data-ttu-id="c212d-121">型</span><span class="sxs-lookup"><span data-stu-id="c212d-121">Type</span></span> | <span data-ttu-id="c212d-122">説明</span><span class="sxs-lookup"><span data-stu-id="c212d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c212d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c212d-123">Authorization</span></span>  | <span data-ttu-id="c212d-124">string</span><span class="sxs-lookup"><span data-stu-id="c212d-124">string</span></span>  | <span data-ttu-id="c212d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c212d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c212d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c212d-127">Content-Type</span></span> | <span data-ttu-id="c212d-128">string</span><span class="sxs-lookup"><span data-stu-id="c212d-128">string</span></span>  | <span data-ttu-id="c212d-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="c212d-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c212d-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c212d-131">Request body</span></span>
<span data-ttu-id="c212d-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c212d-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c212d-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c212d-133">Parameter</span></span>    | <span data-ttu-id="c212d-134">型</span><span class="sxs-lookup"><span data-stu-id="c212d-134">Type</span></span>   |<span data-ttu-id="c212d-135">説明</span><span class="sxs-lookup"><span data-stu-id="c212d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c212d-136">comment</span><span class="sxs-lookup"><span data-stu-id="c212d-136">comment</span></span>|<span data-ttu-id="c212d-137">String</span><span class="sxs-lookup"><span data-stu-id="c212d-137">String</span></span>|<span data-ttu-id="c212d-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c212d-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="c212d-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="c212d-140">toRecipients</span></span>|<span data-ttu-id="c212d-141">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="c212d-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="c212d-142">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c212d-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="c212d-143">応答</span><span class="sxs-lookup"><span data-stu-id="c212d-143">Response</span></span>

<span data-ttu-id="c212d-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c212d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c212d-146">例</span><span class="sxs-lookup"><span data-stu-id="c212d-146">Example</span></span>
<span data-ttu-id="c212d-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c212d-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c212d-148">要求</span><span class="sxs-lookup"><span data-stu-id="c212d-148">Request</span></span>
<span data-ttu-id="c212d-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c212d-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c212d-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c212d-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c212d-151">C#</span><span class="sxs-lookup"><span data-stu-id="c212d-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c212d-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c212d-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c212d-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="c212d-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c212d-154">Java</span><span class="sxs-lookup"><span data-stu-id="c212d-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c212d-155">応答</span><span class="sxs-lookup"><span data-stu-id="c212d-155">Response</span></span>
##### <a name="response"></a><span data-ttu-id="c212d-156">応答</span><span class="sxs-lookup"><span data-stu-id="c212d-156">Response</span></span>
<span data-ttu-id="c212d-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c212d-157">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
