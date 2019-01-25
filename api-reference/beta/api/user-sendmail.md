---
title: メールを送信する
description: 要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afa50b466bd7a90af4fedbdad4c5f7c5b4627b8c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517212"
---
# <a name="send-mail"></a><span data-ttu-id="60b4d-104">メールを送信する</span><span class="sxs-lookup"><span data-stu-id="60b4d-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60b4d-p102">要求本文に指定されたメッセージを送信します。メッセージは、既定で [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="60b4d-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="60b4d-107">同じ**sendMail**のアクションの呼び出しで次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="60b4d-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="60b4d-108">[添付ファイル](../resources/attachment.md)を含める</span><span class="sxs-lookup"><span data-stu-id="60b4d-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="60b4d-109">[説明](../resources/mention.md)を使用して、新しいメッセージに別のユーザーを呼び出す</span><span class="sxs-lookup"><span data-stu-id="60b4d-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="60b4d-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60b4d-110">Permissions</span></span>
<span data-ttu-id="60b4d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60b4d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="60b4d-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60b4d-113">Permission type</span></span>      | <span data-ttu-id="60b4d-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60b4d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60b4d-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60b4d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="60b4d-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="60b4d-116">Mail.Send</span></span>    |
|<span data-ttu-id="60b4d-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60b4d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b4d-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="60b4d-118">Mail.Send</span></span>    |
|<span data-ttu-id="60b4d-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60b4d-119">Application</span></span> | <span data-ttu-id="60b4d-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="60b4d-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="60b4d-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60b4d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="60b4d-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60b4d-122">Request headers</span></span>
| <span data-ttu-id="60b4d-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60b4d-123">Header</span></span>       | <span data-ttu-id="60b4d-124">値</span><span class="sxs-lookup"><span data-stu-id="60b4d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="60b4d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b4d-125">Authorization</span></span>  | <span data-ttu-id="60b4d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60b4d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="60b4d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60b4d-128">Content-Type</span></span>  | <span data-ttu-id="60b4d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="60b4d-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60b4d-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="60b4d-130">Request body</span></span>
<span data-ttu-id="60b4d-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="60b4d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60b4d-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="60b4d-132">Parameter</span></span>    | <span data-ttu-id="60b4d-133">型</span><span class="sxs-lookup"><span data-stu-id="60b4d-133">Type</span></span>   |<span data-ttu-id="60b4d-134">説明</span><span class="sxs-lookup"><span data-stu-id="60b4d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60b4d-135">Message</span><span class="sxs-lookup"><span data-stu-id="60b4d-135">Message</span></span>|[<span data-ttu-id="60b4d-136">Message</span><span class="sxs-lookup"><span data-stu-id="60b4d-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="60b4d-p105">送信するメッセージです。必須。</span><span class="sxs-lookup"><span data-stu-id="60b4d-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="60b4d-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="60b4d-139">SaveToSentItems</span></span>|<span data-ttu-id="60b4d-140">ブール値</span><span class="sxs-lookup"><span data-stu-id="60b4d-140">Boolean</span></span>|<span data-ttu-id="60b4d-p106">[送信済みアイテム] 内のメッセージを保存するかどうかを示します。パラメーターを false にする場合にのみ指定します。既定では true です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="60b4d-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="60b4d-144">**言及**を使用して新しいメッセージに別のユーザーを呼び出す場合は。</span><span class="sxs-lookup"><span data-stu-id="60b4d-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="60b4d-145">要求の本文で必要な**toRecipients**プロパティ**を示して**プロパティ、および任意の書き込み可能なメッセージ プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="60b4d-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="60b4d-146">**紹介**プロパティにそれぞれ記載されている、**記載されている**プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="60b4d-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="60b4d-147">応答</span><span class="sxs-lookup"><span data-stu-id="60b4d-147">Response</span></span>

<span data-ttu-id="60b4d-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="60b4d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60b4d-150">例</span><span class="sxs-lookup"><span data-stu-id="60b4d-150">Example</span></span>
<span data-ttu-id="60b4d-151">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="60b4d-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="60b4d-152">要求 1</span><span class="sxs-lookup"><span data-stu-id="60b4d-152">Request 1</span></span>
<span data-ttu-id="60b4d-153">ここで、作成し、その場でメッセージを送信する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60b4d-153">Here is an example of the request to create and send a message on the fly.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="60b4d-154">応答 1</span><span class="sxs-lookup"><span data-stu-id="60b4d-154">Response 1</span></span>
<span data-ttu-id="60b4d-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="60b4d-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="60b4d-156">要求 2</span><span class="sxs-lookup"><span data-stu-id="60b4d-156">Request 2</span></span>
<span data-ttu-id="60b4d-157">次の例では、彼女のブースにサインインしているユーザーがメッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="60b4d-157">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="60b4d-158">メッセージには、Dana Swope の他のユーザーの参照も含まれています。</span><span class="sxs-lookup"><span data-stu-id="60b4d-158">The message also includes a mention of another user, Dana Swope.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="60b4d-159">応答 2</span><span class="sxs-lookup"><span data-stu-id="60b4d-159">Response 2</span></span>
<span data-ttu-id="60b4d-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="60b4d-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="60b4d-161">要求 3</span><span class="sxs-lookup"><span data-stu-id="60b4d-161">Request 3</span></span>
<span data-ttu-id="60b4d-162">次の例では、カスタムのインターネット メッセージ ヘッダーを持つメッセージを作成し、メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="60b4d-162">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-3"></a><span data-ttu-id="60b4d-163">応答 3</span><span class="sxs-lookup"><span data-stu-id="60b4d-163">Response 3</span></span>
<span data-ttu-id="60b4d-164">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="60b4d-164">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
