---
title: メールを送信する
description: 要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。
author: dkershaw10
ms.openlocfilehash: bceafc0a5142a85acfca59872a9ee897ac839f19
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351766"
---
# <a name="send-mail"></a><span data-ttu-id="04754-104">メールを送信する</span><span class="sxs-lookup"><span data-stu-id="04754-104">Send mail</span></span>

> <span data-ttu-id="04754-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04754-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04754-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04754-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04754-p103">要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="04754-p103">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="04754-109">同じ**sendMail**のアクションの呼び出しで次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="04754-109">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="04754-110">[添付ファイル](../resources/attachment.md)を含める</span><span class="sxs-lookup"><span data-stu-id="04754-110">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="04754-111">[説明](../resources/mention.md)を使用して、新しいメッセージに別のユーザーを呼び出す</span><span class="sxs-lookup"><span data-stu-id="04754-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="04754-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04754-112">Permissions</span></span>
<span data-ttu-id="04754-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04754-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="04754-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04754-115">Permission type</span></span>      | <span data-ttu-id="04754-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04754-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04754-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04754-117">Delegated (work or school account)</span></span> | <span data-ttu-id="04754-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="04754-118">Mail.Send</span></span>    |
|<span data-ttu-id="04754-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04754-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04754-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="04754-120">Mail.Send</span></span>    |
|<span data-ttu-id="04754-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04754-121">Application</span></span> | <span data-ttu-id="04754-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="04754-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="04754-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04754-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="04754-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04754-124">Request headers</span></span>
| <span data-ttu-id="04754-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04754-125">Header</span></span>       | <span data-ttu-id="04754-126">値</span><span class="sxs-lookup"><span data-stu-id="04754-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04754-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="04754-127">Authorization</span></span>  | <span data-ttu-id="04754-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04754-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04754-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04754-130">Content-Type</span></span>  | <span data-ttu-id="04754-131">application/json</span><span class="sxs-lookup"><span data-stu-id="04754-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04754-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="04754-132">Request body</span></span>
<span data-ttu-id="04754-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="04754-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04754-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="04754-134">Parameter</span></span>    | <span data-ttu-id="04754-135">種類</span><span class="sxs-lookup"><span data-stu-id="04754-135">Type</span></span>   |<span data-ttu-id="04754-136">説明</span><span class="sxs-lookup"><span data-stu-id="04754-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04754-137">Message</span><span class="sxs-lookup"><span data-stu-id="04754-137">Message</span></span>|[<span data-ttu-id="04754-138">Message</span><span class="sxs-lookup"><span data-stu-id="04754-138">Message</span></span>](../resources/message.md)|<span data-ttu-id="04754-p106">送信するメッセージです。必須。</span><span class="sxs-lookup"><span data-stu-id="04754-p106">The message to send. Required.</span></span>|
|<span data-ttu-id="04754-141">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="04754-141">SaveToSentItems</span></span>|<span data-ttu-id="04754-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="04754-142">Boolean</span></span>|<span data-ttu-id="04754-p107">[送信済みアイテム] 内のメッセージを保存するかどうかを示します。パラメーターを false にする場合にのみ指定します。既定では true です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="04754-p107">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="04754-146">**言及**を使用して新しいメッセージに別のユーザーを呼び出す場合は。</span><span class="sxs-lookup"><span data-stu-id="04754-146">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="04754-147">要求の本文で必要な**toRecipients**プロパティ**を示して**プロパティ、および任意の書き込み可能なメッセージ プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="04754-147">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="04754-148">**紹介**プロパティにそれぞれ記載されている、**記載されている**プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04754-148">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="04754-149">応答</span><span class="sxs-lookup"><span data-stu-id="04754-149">Response</span></span>

<span data-ttu-id="04754-p108">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="04754-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04754-152">例</span><span class="sxs-lookup"><span data-stu-id="04754-152">Example</span></span>
<span data-ttu-id="04754-153">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="04754-153">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="04754-154">要求 1</span><span class="sxs-lookup"><span data-stu-id="04754-154">Request 1</span></span>
<span data-ttu-id="04754-155">ここで、作成し、その場でメッセージを送信する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04754-155">Here is an example of the request to create and send a message on the fly.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 512

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
          "address": "samanthab@contoso.onmicrosoft.com"
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

##### <a name="response-1"></a><span data-ttu-id="04754-156">応答 1</span><span class="sxs-lookup"><span data-stu-id="04754-156">Response 1</span></span>
<span data-ttu-id="04754-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="04754-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="04754-158">要求 2</span><span class="sxs-lookup"><span data-stu-id="04754-158">Request 2</span></span>
<span data-ttu-id="04754-159">次の例では、彼女のブースにサインインしているユーザーがメッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="04754-159">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="04754-160">メッセージには、Dana Swope の他のユーザーの参照も含まれています。</span><span class="sxs-lookup"><span data-stu-id="04754-160">The message also includes a mention of another user, Dana Swope.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_mentions"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 344

{
  "Message": {
    "subject": "Project kickoff",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
  }
}
```

##### <a name="response-2"></a><span data-ttu-id="04754-161">応答 2</span><span class="sxs-lookup"><span data-stu-id="04754-161">Response 2</span></span>
<span data-ttu-id="04754-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="04754-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="04754-163">要求 3</span><span class="sxs-lookup"><span data-stu-id="04754-163">Request 3</span></span>
<span data-ttu-id="04754-164">次の例では、カスタムのインターネット メッセージ ヘッダーを持つメッセージを作成し、メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="04754-164">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
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

##### <a name="response-3"></a><span data-ttu-id="04754-165">応答 3</span><span class="sxs-lookup"><span data-stu-id="04754-165">Response 3</span></span>
<span data-ttu-id="04754-166">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="04754-166">Here is an example of the response.</span></span>
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
