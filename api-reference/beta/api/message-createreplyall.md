---
title: 'メッセージ: createReplyAll'
description: 'コメントを含めるか、メッセージのプロパティを更新するすべての返信メッセージの下書きを作成します。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8d42517daa5c8242f28c6dfb3cb4d508b2667ed5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528579"
---
# <a name="message-createreplyall"></a><span data-ttu-id="0ebca-103">メッセージ: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="0ebca-103">message: createReplyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ebca-p101">1 回の createReplyAll 呼び出しで下書きの全員に返信メッセージを作成して、コメントを含めるかメッセージのプロパティを更新します。その後、下書きを 更新 または 送信 できます。</span><span class="sxs-lookup"><span data-stu-id="0ebca-p101">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="0ebca-106">**注**</span><span class="sxs-lookup"><span data-stu-id="0ebca-106">**Note**</span></span>

- <span data-ttu-id="0ebca-p102">コメントまたは `message` パラメーターの **Body** プロパティを指定できます。両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="0ebca-p102">You can specify either a comment or the **body** property of the `message` parameter. Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="0ebca-109">**ReplyTo**プロパティが元のメッセージのインターネット メッセージ フォーマット ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに指定されている場合は、内の受信者に返信を送信する必要があります、</span><span class="sxs-lookup"><span data-stu-id="0ebca-109">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="0ebca-110">**replyTo**と**toRecipients**プロパティと**から**と**toRecipients**プロパティで受信者ではありません。</span><span class="sxs-lookup"><span data-stu-id="0ebca-110">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0ebca-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0ebca-111">Permissions</span></span>
<span data-ttu-id="0ebca-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ebca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ebca-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ebca-114">Permission type</span></span>      | <span data-ttu-id="0ebca-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ebca-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ebca-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ebca-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0ebca-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ebca-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ebca-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ebca-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ebca-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ebca-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ebca-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ebca-120">Application</span></span> | <span data-ttu-id="0ebca-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ebca-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ebca-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ebca-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="0ebca-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ebca-123">Request headers</span></span>
| <span data-ttu-id="0ebca-124">名前</span><span class="sxs-lookup"><span data-stu-id="0ebca-124">Name</span></span>       | <span data-ttu-id="0ebca-125">型</span><span class="sxs-lookup"><span data-stu-id="0ebca-125">Type</span></span> | <span data-ttu-id="0ebca-126">説明</span><span class="sxs-lookup"><span data-stu-id="0ebca-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ebca-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ebca-127">Authorization</span></span>  | <span data-ttu-id="0ebca-128">string</span><span class="sxs-lookup"><span data-stu-id="0ebca-128">string</span></span>  | <span data-ttu-id="0ebca-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0ebca-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ebca-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ebca-131">Content-Type</span></span> | <span data-ttu-id="0ebca-132">string</span><span class="sxs-lookup"><span data-stu-id="0ebca-132">string</span></span>  | <span data-ttu-id="0ebca-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="0ebca-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ebca-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ebca-135">Request body</span></span>
<span data-ttu-id="0ebca-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0ebca-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ebca-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0ebca-137">Parameter</span></span>    | <span data-ttu-id="0ebca-138">型</span><span class="sxs-lookup"><span data-stu-id="0ebca-138">Type</span></span>   |<span data-ttu-id="0ebca-139">説明</span><span class="sxs-lookup"><span data-stu-id="0ebca-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ebca-140">comment</span><span class="sxs-lookup"><span data-stu-id="0ebca-140">comment</span></span>|<span data-ttu-id="0ebca-141">String</span><span class="sxs-lookup"><span data-stu-id="0ebca-141">String</span></span>|<span data-ttu-id="0ebca-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0ebca-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="0ebca-144">message</span><span class="sxs-lookup"><span data-stu-id="0ebca-144">message</span></span>|[<span data-ttu-id="0ebca-145">message</span><span class="sxs-lookup"><span data-stu-id="0ebca-145">message</span></span>](../resources/message.md)|<span data-ttu-id="0ebca-146">全員に返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="0ebca-146">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="0ebca-147">応答</span><span class="sxs-lookup"><span data-stu-id="0ebca-147">Response</span></span>

<span data-ttu-id="0ebca-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0ebca-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ebca-149">例</span><span class="sxs-lookup"><span data-stu-id="0ebca-149">Example</span></span>
<span data-ttu-id="0ebca-150">次の例では、1 回の **CreateReplyAll** 呼び出しで全員に返信する下書きを作成し、添付ファイルをコメントに追加します。</span><span class="sxs-lookup"><span data-stu-id="0ebca-150">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="0ebca-151">要求</span><span class="sxs-lookup"><span data-stu-id="0ebca-151">Request</span></span>
<span data-ttu-id="0ebca-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ebca-152">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0ebca-153">応答</span><span class="sxs-lookup"><span data-stu-id="0ebca-153">Response</span></span>
<span data-ttu-id="0ebca-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ebca-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-createreplyall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
