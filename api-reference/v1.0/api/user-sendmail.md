---
title: メールを送信する
description: 要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。
author: dkershaw10
ms.openlocfilehash: a818ec5cc455b6ca78c920be57ad34155a03a1bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333293"
---
# <a name="send-mail"></a><span data-ttu-id="e0fef-104">メールを送信する</span><span class="sxs-lookup"><span data-stu-id="e0fef-104">Send mail</span></span>

<span data-ttu-id="e0fef-p102">要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="e0fef-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="e0fef-107">[添付ファイル](../resources/fileattachment.md)を同じ **sendMail** アクション呼び出しに含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e0fef-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0fef-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e0fef-108">Permissions</span></span>
<span data-ttu-id="e0fef-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0fef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e0fef-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0fef-111">Permission type</span></span>      | <span data-ttu-id="e0fef-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0fef-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0fef-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0fef-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e0fef-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e0fef-114">Mail.Send</span></span>    |
|<span data-ttu-id="e0fef-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0fef-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0fef-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e0fef-116">Mail.Send</span></span>    |
|<span data-ttu-id="e0fef-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0fef-117">Application</span></span> | <span data-ttu-id="e0fef-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e0fef-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0fef-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0fef-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="e0fef-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0fef-120">Request headers</span></span>
| <span data-ttu-id="e0fef-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0fef-121">Header</span></span>       | <span data-ttu-id="e0fef-122">値</span><span class="sxs-lookup"><span data-stu-id="e0fef-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0fef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0fef-123">Authorization</span></span>  | <span data-ttu-id="e0fef-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e0fef-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0fef-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0fef-126">Content-Type</span></span>  | <span data-ttu-id="e0fef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e0fef-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0fef-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0fef-128">Request body</span></span>
<span data-ttu-id="e0fef-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0fef-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0fef-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e0fef-130">Parameter</span></span>    | <span data-ttu-id="e0fef-131">種類</span><span class="sxs-lookup"><span data-stu-id="e0fef-131">Type</span></span>   |<span data-ttu-id="e0fef-132">説明</span><span class="sxs-lookup"><span data-stu-id="e0fef-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0fef-133">message</span><span class="sxs-lookup"><span data-stu-id="e0fef-133">message</span></span>|[<span data-ttu-id="e0fef-134">Message</span><span class="sxs-lookup"><span data-stu-id="e0fef-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="e0fef-p105">送信するメッセージです。必須。</span><span class="sxs-lookup"><span data-stu-id="e0fef-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="e0fef-137">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="e0fef-137">saveToSentItems</span></span>|<span data-ttu-id="e0fef-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0fef-138">Boolean</span></span>|<span data-ttu-id="e0fef-p106">[送信済みアイテム] 内のメッセージを保存するかどうかを示します。パラメーターを false にする場合にのみ指定します。既定では true です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e0fef-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e0fef-142">応答</span><span class="sxs-lookup"><span data-stu-id="e0fef-142">Response</span></span>

<span data-ttu-id="e0fef-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e0fef-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0fef-145">例</span><span class="sxs-lookup"><span data-stu-id="e0fef-145">Example</span></span>
<span data-ttu-id="e0fef-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e0fef-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="e0fef-147">要求 1</span><span class="sxs-lookup"><span data-stu-id="e0fef-147">Request 1</span></span>
<span data-ttu-id="e0fef-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0fef-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <a name="response-1"></a><span data-ttu-id="e0fef-149">応答 1</span><span class="sxs-lookup"><span data-stu-id="e0fef-149">Response 1</span></span>
<span data-ttu-id="e0fef-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e0fef-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="e0fef-151">要求 2</span><span class="sxs-lookup"><span data-stu-id="e0fef-151">Request 2</span></span>
<span data-ttu-id="e0fef-152">次の例では、カスタムのインターネット メッセージ ヘッダーを持つメッセージを作成し、メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="e0fef-152">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "9/9/2018: concert",
    "body": {
      "contentType": "HTML",
      "content": "The group represents Nevada."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    ],
    "internetMessageHeaders":[
      {
        "name":"x-custom-header-group-name",
        "value":"Nevada"
      },
      {
        "name":"x-custom-header-group-id",
        "value":"NV001"
      }
    ]
  }
}
```

##### <a name="response-2"></a><span data-ttu-id="e0fef-153">応答 2</span><span class="sxs-lookup"><span data-stu-id="e0fef-153">Response 2</span></span>
<span data-ttu-id="e0fef-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e0fef-154">Here is an example of the response.</span></span>
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
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
