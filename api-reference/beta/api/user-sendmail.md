---
title: メールを送信する
description: 要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 806dbeff7540be3d31d63e9f685d797feb266650
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325912"
---
# <a name="send-mail"></a><span data-ttu-id="27141-104">メールを送信する</span><span class="sxs-lookup"><span data-stu-id="27141-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27141-p102">要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="27141-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="27141-107">同じ**sendMail**アクション呼び出しでは、次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="27141-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="27141-108">[添付ファイル](../resources/attachment.md)を含める</span><span class="sxs-lookup"><span data-stu-id="27141-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="27141-109">別のユーザーを新しいメッセージで呼び出すには、[メンション](../resources/mention.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="27141-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="27141-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="27141-110">Permissions</span></span>
<span data-ttu-id="27141-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27141-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="27141-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27141-113">Permission type</span></span>      | <span data-ttu-id="27141-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="27141-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27141-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27141-115">Delegated (work or school account)</span></span> | <span data-ttu-id="27141-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="27141-116">Mail.Send</span></span>    |
|<span data-ttu-id="27141-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27141-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27141-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="27141-118">Mail.Send</span></span>    |
|<span data-ttu-id="27141-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27141-119">Application</span></span> | <span data-ttu-id="27141-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="27141-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="27141-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27141-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="27141-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27141-122">Request headers</span></span>
| <span data-ttu-id="27141-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27141-123">Header</span></span>       | <span data-ttu-id="27141-124">値</span><span class="sxs-lookup"><span data-stu-id="27141-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27141-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="27141-125">Authorization</span></span>  | <span data-ttu-id="27141-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="27141-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27141-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27141-128">Content-Type</span></span>  | <span data-ttu-id="27141-129">application/json</span><span class="sxs-lookup"><span data-stu-id="27141-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27141-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="27141-130">Request body</span></span>
<span data-ttu-id="27141-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="27141-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="27141-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="27141-132">Parameter</span></span>    | <span data-ttu-id="27141-133">型</span><span class="sxs-lookup"><span data-stu-id="27141-133">Type</span></span>   |<span data-ttu-id="27141-134">説明</span><span class="sxs-lookup"><span data-stu-id="27141-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27141-135">メッセージ</span><span class="sxs-lookup"><span data-stu-id="27141-135">Message</span></span>|[<span data-ttu-id="27141-136">Message</span><span class="sxs-lookup"><span data-stu-id="27141-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="27141-p105">送信するメッセージです。必須。</span><span class="sxs-lookup"><span data-stu-id="27141-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="27141-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="27141-139">SaveToSentItems</span></span>|<span data-ttu-id="27141-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="27141-140">Boolean</span></span>|<span data-ttu-id="27141-p106">[送信済みアイテム] 内のメッセージを保存するかどうかを示します。パラメーターを false にする場合にのみ指定します。既定では true です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="27141-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="27141-144">新しいメッセージで別のユーザーを呼び出すために、**メンション**を使用する場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="27141-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="27141-145">要求本文に、必要な**Torecipients**プロパティ、**メンション**プロパティ、および任意の書き込み可能なメッセージプロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="27141-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="27141-146">**メンション**プロパティの各メンションに対して、**説明**されているプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="27141-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="27141-147">応答</span><span class="sxs-lookup"><span data-stu-id="27141-147">Response</span></span>

<span data-ttu-id="27141-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="27141-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27141-150">例</span><span class="sxs-lookup"><span data-stu-id="27141-150">Example</span></span>
<span data-ttu-id="27141-151">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="27141-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="27141-152">要求 1</span><span class="sxs-lookup"><span data-stu-id="27141-152">Request 1</span></span>
<span data-ttu-id="27141-153">ここでは、メッセージを作成してその場で送信する要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="27141-153">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27141-154">プロトコル</span><span class="sxs-lookup"><span data-stu-id="27141-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="27141-155">C#</span><span class="sxs-lookup"><span data-stu-id="27141-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27141-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27141-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27141-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="27141-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="27141-158">Java</span><span class="sxs-lookup"><span data-stu-id="27141-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="27141-159">応答 1</span><span class="sxs-lookup"><span data-stu-id="27141-159">Response 1</span></span>
<span data-ttu-id="27141-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="27141-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="27141-161">要求 2</span><span class="sxs-lookup"><span data-stu-id="27141-161">Request 2</span></span>
<span data-ttu-id="27141-162">次の例は、サインインしているユーザーが Samantha ブースにメッセージを表示しています。</span><span class="sxs-lookup"><span data-stu-id="27141-162">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="27141-163">このメッセージには、別のユーザーの Dana Swope も含まれています。</span><span class="sxs-lookup"><span data-stu-id="27141-163">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27141-164">プロトコル</span><span class="sxs-lookup"><span data-stu-id="27141-164">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="27141-165">C#</span><span class="sxs-lookup"><span data-stu-id="27141-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27141-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27141-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27141-167">目的-C</span><span class="sxs-lookup"><span data-stu-id="27141-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="27141-168">Java</span><span class="sxs-lookup"><span data-stu-id="27141-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="27141-169">応答 2</span><span class="sxs-lookup"><span data-stu-id="27141-169">Response 2</span></span>
<span data-ttu-id="27141-170">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="27141-170">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="27141-171">要求 3</span><span class="sxs-lookup"><span data-stu-id="27141-171">Request 3</span></span>
<span data-ttu-id="27141-172">次の例では、カスタムのインターネット メッセージ ヘッダーでメッセージを作成し、送信します。</span><span class="sxs-lookup"><span data-stu-id="27141-172">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27141-173">プロトコル</span><span class="sxs-lookup"><span data-stu-id="27141-173">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="27141-174">C#</span><span class="sxs-lookup"><span data-stu-id="27141-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27141-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27141-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27141-176">目的-C</span><span class="sxs-lookup"><span data-stu-id="27141-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="27141-177">Java</span><span class="sxs-lookup"><span data-stu-id="27141-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="27141-178">応答 3</span><span class="sxs-lookup"><span data-stu-id="27141-178">Response 3</span></span>
<span data-ttu-id="27141-179">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="27141-179">Here is an example of the response.</span></span>
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
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
