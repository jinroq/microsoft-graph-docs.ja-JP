---
title: 'メッセージ: createReply'
description: 'コメントを含めるか、メッセージ ・ プロパティの更新への返信メッセージの下書きを作成します。 '
ms.openlocfilehash: 40bdd5792e9d7a018fc8c7b1aca2d5955a8ef807
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073634"
---
# <a name="message-createreply"></a><span data-ttu-id="be8bb-103">メッセージ: createReply</span><span class="sxs-lookup"><span data-stu-id="be8bb-103">message: createReply</span></span>

> <span data-ttu-id="be8bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="be8bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be8bb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be8bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be8bb-p102">1 回の **createReply** 呼び出しで下書きの返信メッセージを作成して、コメントを含めるかメッセージのプロパティを更新します。その後、下書きを [更新](../api/message-update.md) または [送信](../api/message-send.md) できます。</span><span class="sxs-lookup"><span data-stu-id="be8bb-p102">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="be8bb-108">**メモ**</span><span class="sxs-lookup"><span data-stu-id="be8bb-108">**Note**</span></span>

- <span data-ttu-id="be8bb-109">**Body**プロパティまたはコメントのいずれかを指定することができます、`message`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="be8bb-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="be8bb-110">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="be8bb-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="be8bb-111">**ReplyTo**が元のメッセージのインターネット メッセージ フォーマット ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに指定されている場合**から**の**replyTo**、内の受信者と受信者ではありませんへの返信を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="be8bb-111">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="be8bb-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be8bb-112">Permissions</span></span>
<span data-ttu-id="be8bb-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be8bb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be8bb-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be8bb-115">Permission type</span></span>      | <span data-ttu-id="be8bb-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be8bb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be8bb-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be8bb-117">Delegated (work or school account)</span></span> | <span data-ttu-id="be8bb-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be8bb-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="be8bb-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be8bb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be8bb-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be8bb-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="be8bb-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be8bb-121">Application</span></span> | <span data-ttu-id="be8bb-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be8bb-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="be8bb-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be8bb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="be8bb-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be8bb-124">Request headers</span></span>
| <span data-ttu-id="be8bb-125">名前</span><span class="sxs-lookup"><span data-stu-id="be8bb-125">Name</span></span>       | <span data-ttu-id="be8bb-126">型</span><span class="sxs-lookup"><span data-stu-id="be8bb-126">Type</span></span> | <span data-ttu-id="be8bb-127">説明</span><span class="sxs-lookup"><span data-stu-id="be8bb-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="be8bb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="be8bb-128">Authorization</span></span>  | <span data-ttu-id="be8bb-129">string</span><span class="sxs-lookup"><span data-stu-id="be8bb-129">string</span></span>  | <span data-ttu-id="be8bb-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be8bb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be8bb-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be8bb-132">Content-Type</span></span> | <span data-ttu-id="be8bb-133">string</span><span class="sxs-lookup"><span data-stu-id="be8bb-133">string</span></span>  | <span data-ttu-id="be8bb-p106">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="be8bb-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be8bb-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="be8bb-136">Request body</span></span>
<span data-ttu-id="be8bb-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="be8bb-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="be8bb-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="be8bb-138">Parameter</span></span>    | <span data-ttu-id="be8bb-139">型</span><span class="sxs-lookup"><span data-stu-id="be8bb-139">Type</span></span>   |<span data-ttu-id="be8bb-140">説明</span><span class="sxs-lookup"><span data-stu-id="be8bb-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be8bb-141">comment</span><span class="sxs-lookup"><span data-stu-id="be8bb-141">comment</span></span>|<span data-ttu-id="be8bb-142">String</span><span class="sxs-lookup"><span data-stu-id="be8bb-142">String</span></span>|<span data-ttu-id="be8bb-p107">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="be8bb-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="be8bb-145">message</span><span class="sxs-lookup"><span data-stu-id="be8bb-145">message</span></span>|[<span data-ttu-id="be8bb-146">message</span><span class="sxs-lookup"><span data-stu-id="be8bb-146">message</span></span>](../resources/message.md)|<span data-ttu-id="be8bb-147">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="be8bb-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="be8bb-148">応答</span><span class="sxs-lookup"><span data-stu-id="be8bb-148">Response</span></span>

<span data-ttu-id="be8bb-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be8bb-149">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be8bb-150">例</span><span class="sxs-lookup"><span data-stu-id="be8bb-150">Example</span></span>
<span data-ttu-id="be8bb-151">次の例では、下書きの返信を作成し、要求の本文にコメントと受信者を追加します。</span><span class="sxs-lookup"><span data-stu-id="be8bb-151">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="be8bb-152">要求</span><span class="sxs-lookup"><span data-stu-id="be8bb-152">Request</span></span>
<span data-ttu-id="be8bb-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be8bb-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group if the project is approved, please?" 
}
```

##### <a name="response"></a><span data-ttu-id="be8bb-154">応答</span><span class="sxs-lookup"><span data-stu-id="be8bb-154">Response</span></span>
<span data-ttu-id="be8bb-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be8bb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKoAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DO\"",
  "id": "AAMkADA1MTAAAH5JKoAAA=",
  "subject": "RE: Let's start a group",
  "Body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>Samantha, Randi, would you name the group if the project is approved, please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n<p>That's a great idea!<br>\r\n</body>\r\n</html>"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress": {
        "name": "Randi Welch",
        "address": "randiw@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
