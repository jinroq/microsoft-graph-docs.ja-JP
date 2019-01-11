---
title: 'メッセージ: createReplyAll'
description: 'コメントを含めるか、メッセージのプロパティを更新するすべての返信メッセージの下書きを作成します。 '
localization_priority: Normal
ms.openlocfilehash: 2d56f79b415232954434841d89cbdc95bafc1c6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816927"
---
# <a name="message-createreplyall"></a><span data-ttu-id="7d9de-103">メッセージ: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="7d9de-103">message: createReplyAll</span></span>

> <span data-ttu-id="7d9de-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d9de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d9de-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d9de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d9de-p102">1 回の **createReplyAll** 呼び出しで下書きの全員に返信メッセージを作成して、コメントを含めるかメッセージのプロパティを更新します。その後、下書きを [更新](../api/message-update.md) または [送信](../api/message-send.md) できます。</span><span class="sxs-lookup"><span data-stu-id="7d9de-p102">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="7d9de-108">**注**</span><span class="sxs-lookup"><span data-stu-id="7d9de-108">**Note**</span></span>

- <span data-ttu-id="7d9de-109">**Body**プロパティまたはコメントのいずれかを指定することができます、`message`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="7d9de-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="7d9de-110">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="7d9de-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="7d9de-111">**ReplyTo**プロパティが元のメッセージのインターネット メッセージ フォーマット ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに指定されている場合は、内の受信者に返信を送信する必要があります、</span><span class="sxs-lookup"><span data-stu-id="7d9de-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="7d9de-112">**replyTo**と**toRecipients**プロパティと**から**と**toRecipients**プロパティで受信者ではありません。</span><span class="sxs-lookup"><span data-stu-id="7d9de-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7d9de-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d9de-113">Permissions</span></span>
<span data-ttu-id="7d9de-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d9de-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d9de-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d9de-116">Permission type</span></span>      | <span data-ttu-id="7d9de-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d9de-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d9de-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d9de-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7d9de-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d9de-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7d9de-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d9de-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d9de-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d9de-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7d9de-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d9de-122">Application</span></span> | <span data-ttu-id="7d9de-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d9de-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d9de-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d9de-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="7d9de-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d9de-125">Request headers</span></span>
| <span data-ttu-id="7d9de-126">名前</span><span class="sxs-lookup"><span data-stu-id="7d9de-126">Name</span></span>       | <span data-ttu-id="7d9de-127">種類</span><span class="sxs-lookup"><span data-stu-id="7d9de-127">Type</span></span> | <span data-ttu-id="7d9de-128">説明</span><span class="sxs-lookup"><span data-stu-id="7d9de-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d9de-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d9de-129">Authorization</span></span>  | <span data-ttu-id="7d9de-130">string</span><span class="sxs-lookup"><span data-stu-id="7d9de-130">string</span></span>  | <span data-ttu-id="7d9de-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d9de-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d9de-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d9de-133">Content-Type</span></span> | <span data-ttu-id="7d9de-134">string</span><span class="sxs-lookup"><span data-stu-id="7d9de-134">string</span></span>  | <span data-ttu-id="7d9de-p106">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="7d9de-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d9de-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d9de-137">Request body</span></span>
<span data-ttu-id="7d9de-138">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d9de-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d9de-139">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7d9de-139">Parameter</span></span>    | <span data-ttu-id="7d9de-140">Type</span><span class="sxs-lookup"><span data-stu-id="7d9de-140">Type</span></span>   |<span data-ttu-id="7d9de-141">説明</span><span class="sxs-lookup"><span data-stu-id="7d9de-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d9de-142">comment</span><span class="sxs-lookup"><span data-stu-id="7d9de-142">comment</span></span>|<span data-ttu-id="7d9de-143">String</span><span class="sxs-lookup"><span data-stu-id="7d9de-143">String</span></span>|<span data-ttu-id="7d9de-p107">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7d9de-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="7d9de-146">message</span><span class="sxs-lookup"><span data-stu-id="7d9de-146">message</span></span>|[<span data-ttu-id="7d9de-147">message</span><span class="sxs-lookup"><span data-stu-id="7d9de-147">message</span></span>](../resources/message.md)|<span data-ttu-id="7d9de-148">全員に返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="7d9de-148">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="7d9de-149">応答</span><span class="sxs-lookup"><span data-stu-id="7d9de-149">Response</span></span>

<span data-ttu-id="7d9de-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d9de-150">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d9de-151">例</span><span class="sxs-lookup"><span data-stu-id="7d9de-151">Example</span></span>
<span data-ttu-id="7d9de-152">次の使用例は、全員に返信するのには下書きを作成し、1 つの**createReplyAll**呼び出しですべての添付ファイルとコメントを追加します。</span><span class="sxs-lookup"><span data-stu-id="7d9de-152">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="7d9de-153">要求</span><span class="sxs-lookup"><span data-stu-id="7d9de-153">Request</span></span>
<span data-ttu-id="7d9de-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d9de-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
}
```

##### <a name="response"></a><span data-ttu-id="7d9de-155">応答</span><span class="sxs-lookup"><span data-stu-id="7d9de-155">Response</span></span>
<span data-ttu-id="7d9de-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d9de-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKpAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DP\"",
  "id": "AAMkADA1MTAAAH5JKpAAA=",
  "subject": "RE: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body dir=\"ltr\">\r\nif the project gets approved, please take a look at the attached guidelines before you decide on the name.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:36:32 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group\r\n<div>Samantha, Randi, would you name the group please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n</body>\r\n</html>"
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
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
