---
title: 'メッセージ: createReplyAll'
description: '全員に返信メッセージの下書きを作成してコメントを含めるか、メッセージのプロパティを更新します。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: fdfe2287ffbdb8d99b7742d1cbc9488fa2b2a3ad
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448265"
---
# <a name="message-createreplyall"></a><span data-ttu-id="f3cd2-103">メッセージ: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="f3cd2-103">message: createReplyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3cd2-p101">1 回の createReplyAll 呼び出しで下書きの全員に返信メッセージを作成して、コメントを含めるかメッセージのプロパティを更新します。その後、下書きを 更新 または 送信 できます。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-p101">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="f3cd2-106">**注**</span><span class="sxs-lookup"><span data-stu-id="f3cd2-106">**Note**</span></span>

- <span data-ttu-id="f3cd2-107">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="f3cd2-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="f3cd2-108">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="f3cd2-109">元のメッセージで**replyTo**プロパティが指定されている場合、インターネットメッセージ形式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに、受信者に返信を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-109">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="f3cd2-110">**replyTo**プロパティ\*\*\*\* と torプロパティのプロパティ。これは、 **from**および**torの piの**各プロパティの受信者ではありません。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-110">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="f3cd2-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3cd2-111">Permissions</span></span>
<span data-ttu-id="f3cd2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3cd2-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3cd2-114">Permission type</span></span>      | <span data-ttu-id="f3cd2-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3cd2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3cd2-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3cd2-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f3cd2-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3cd2-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f3cd2-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3cd2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3cd2-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3cd2-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f3cd2-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3cd2-120">Application</span></span> | <span data-ttu-id="f3cd2-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3cd2-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3cd2-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3cd2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="f3cd2-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3cd2-123">Request headers</span></span>
| <span data-ttu-id="f3cd2-124">名前</span><span class="sxs-lookup"><span data-stu-id="f3cd2-124">Name</span></span>       | <span data-ttu-id="f3cd2-125">型</span><span class="sxs-lookup"><span data-stu-id="f3cd2-125">Type</span></span> | <span data-ttu-id="f3cd2-126">説明</span><span class="sxs-lookup"><span data-stu-id="f3cd2-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f3cd2-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3cd2-127">Authorization</span></span>  | <span data-ttu-id="f3cd2-128">string</span><span class="sxs-lookup"><span data-stu-id="f3cd2-128">string</span></span>  | <span data-ttu-id="f3cd2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3cd2-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f3cd2-131">Content-Type</span></span> | <span data-ttu-id="f3cd2-132">string</span><span class="sxs-lookup"><span data-stu-id="f3cd2-132">string</span></span>  | <span data-ttu-id="f3cd2-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3cd2-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3cd2-135">Request body</span></span>
<span data-ttu-id="f3cd2-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f3cd2-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f3cd2-137">Parameter</span></span>    | <span data-ttu-id="f3cd2-138">型</span><span class="sxs-lookup"><span data-stu-id="f3cd2-138">Type</span></span>   |<span data-ttu-id="f3cd2-139">説明</span><span class="sxs-lookup"><span data-stu-id="f3cd2-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3cd2-140">comment</span><span class="sxs-lookup"><span data-stu-id="f3cd2-140">comment</span></span>|<span data-ttu-id="f3cd2-141">String</span><span class="sxs-lookup"><span data-stu-id="f3cd2-141">String</span></span>|<span data-ttu-id="f3cd2-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f3cd2-144">message</span><span class="sxs-lookup"><span data-stu-id="f3cd2-144">message</span></span>|[<span data-ttu-id="f3cd2-145">message</span><span class="sxs-lookup"><span data-stu-id="f3cd2-145">message</span></span>](../resources/message.md)|<span data-ttu-id="f3cd2-146">全員に返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-146">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="f3cd2-147">応答</span><span class="sxs-lookup"><span data-stu-id="f3cd2-147">Response</span></span>

<span data-ttu-id="f3cd2-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3cd2-149">例</span><span class="sxs-lookup"><span data-stu-id="f3cd2-149">Example</span></span>
<span data-ttu-id="f3cd2-150">次の例では、全員に返信する下書きを作成し、1つの**Createreplyall**呼び出しで添付ファイルとコメントをすべて追加します。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-150">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="f3cd2-151">要求</span><span class="sxs-lookup"><span data-stu-id="f3cd2-151">Request</span></span>
<span data-ttu-id="f3cd2-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-152">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f3cd2-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f3cd2-153">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f3cd2-154">C#</span><span class="sxs-lookup"><span data-stu-id="f3cd2-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3cd2-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="f3cd2-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f3cd2-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="f3cd2-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f3cd2-157">応答</span><span class="sxs-lookup"><span data-stu-id="f3cd2-157">Response</span></span>
<span data-ttu-id="f3cd2-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3cd2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
