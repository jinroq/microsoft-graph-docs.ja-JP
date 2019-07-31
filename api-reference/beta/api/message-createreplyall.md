---
title: 'メッセージ: createReplyAll'
description: '全員に返信メッセージの下書きを作成してコメントを含めるか、メッセージのプロパティを更新します。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 38c61608f080e336b239685476bf3b3d354643c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983928"
---
# <a name="message-createreplyall"></a><span data-ttu-id="f90de-103">メッセージ: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="f90de-103">message: createReplyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f90de-p101">1 回の createReplyAll 呼び出しで下書きの全員に返信メッセージを作成して、コメントを含めるかメッセージのプロパティを更新します。その後、下書きを 更新 または 送信 できます。</span><span class="sxs-lookup"><span data-stu-id="f90de-p101">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="f90de-106">**注**</span><span class="sxs-lookup"><span data-stu-id="f90de-106">**Note**</span></span>

- <span data-ttu-id="f90de-107">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="f90de-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="f90de-108">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="f90de-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="f90de-109">元のメッセージで**replyTo**プロパティが指定されている場合、インターネットメッセージ形式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに、受信者に返信を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f90de-109">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="f90de-110">**replyTo**プロパティ\*\*\*\* と torプロパティのプロパティ。これは、 **from**および**torの piの**各プロパティの受信者ではありません。</span><span class="sxs-lookup"><span data-stu-id="f90de-110">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="f90de-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f90de-111">Permissions</span></span>
<span data-ttu-id="f90de-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f90de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f90de-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f90de-114">Permission type</span></span>      | <span data-ttu-id="f90de-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f90de-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f90de-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f90de-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f90de-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f90de-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f90de-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f90de-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f90de-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f90de-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f90de-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f90de-120">Application</span></span> | <span data-ttu-id="f90de-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f90de-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f90de-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f90de-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="f90de-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f90de-123">Request headers</span></span>
| <span data-ttu-id="f90de-124">名前</span><span class="sxs-lookup"><span data-stu-id="f90de-124">Name</span></span>       | <span data-ttu-id="f90de-125">型</span><span class="sxs-lookup"><span data-stu-id="f90de-125">Type</span></span> | <span data-ttu-id="f90de-126">説明</span><span class="sxs-lookup"><span data-stu-id="f90de-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f90de-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f90de-127">Authorization</span></span>  | <span data-ttu-id="f90de-128">string</span><span class="sxs-lookup"><span data-stu-id="f90de-128">string</span></span>  | <span data-ttu-id="f90de-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f90de-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f90de-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f90de-131">Content-Type</span></span> | <span data-ttu-id="f90de-132">string</span><span class="sxs-lookup"><span data-stu-id="f90de-132">string</span></span>  | <span data-ttu-id="f90de-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="f90de-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f90de-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="f90de-135">Request body</span></span>
<span data-ttu-id="f90de-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f90de-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f90de-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f90de-137">Parameter</span></span>    | <span data-ttu-id="f90de-138">型</span><span class="sxs-lookup"><span data-stu-id="f90de-138">Type</span></span>   |<span data-ttu-id="f90de-139">説明</span><span class="sxs-lookup"><span data-stu-id="f90de-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f90de-140">comment</span><span class="sxs-lookup"><span data-stu-id="f90de-140">comment</span></span>|<span data-ttu-id="f90de-141">String</span><span class="sxs-lookup"><span data-stu-id="f90de-141">String</span></span>|<span data-ttu-id="f90de-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f90de-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f90de-144">message</span><span class="sxs-lookup"><span data-stu-id="f90de-144">message</span></span>|[<span data-ttu-id="f90de-145">message</span><span class="sxs-lookup"><span data-stu-id="f90de-145">message</span></span>](../resources/message.md)|<span data-ttu-id="f90de-146">全員に返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="f90de-146">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="f90de-147">応答</span><span class="sxs-lookup"><span data-stu-id="f90de-147">Response</span></span>

<span data-ttu-id="f90de-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f90de-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f90de-149">例</span><span class="sxs-lookup"><span data-stu-id="f90de-149">Example</span></span>
<span data-ttu-id="f90de-150">次の例では、全員に返信する下書きを作成し、1つの**Createreplyall**呼び出しで添付ファイルとコメントをすべて追加します。</span><span class="sxs-lookup"><span data-stu-id="f90de-150">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="f90de-151">要求</span><span class="sxs-lookup"><span data-stu-id="f90de-151">Request</span></span>
<span data-ttu-id="f90de-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f90de-152">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f90de-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f90de-153">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f90de-154">C#</span><span class="sxs-lookup"><span data-stu-id="f90de-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f90de-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="f90de-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f90de-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="f90de-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f90de-157">Java</span><span class="sxs-lookup"><span data-stu-id="f90de-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f90de-158">応答</span><span class="sxs-lookup"><span data-stu-id="f90de-158">Response</span></span>
<span data-ttu-id="f90de-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f90de-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
