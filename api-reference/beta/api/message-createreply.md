---
title: 'メッセージ: createReply'
description: '返信メッセージの下書きを作成してコメントを含めるか、メッセージのプロパティを更新する '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b24011e377fca25343096d6729c4f68ea3179996
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992928"
---
# <a name="message-createreply"></a><span data-ttu-id="53795-103">メッセージ: createReply</span><span class="sxs-lookup"><span data-stu-id="53795-103">message: createReply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53795-p101">1 回の createReply 呼び出しで下書きの返信メッセージを作成して、コメントを含めるかメッセージのプロパティを更新します。その後、下書きを 更新 または 送信 できます。</span><span class="sxs-lookup"><span data-stu-id="53795-p101">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="53795-106">**注**</span><span class="sxs-lookup"><span data-stu-id="53795-106">**Note**</span></span>

- <span data-ttu-id="53795-107">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="53795-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="53795-108">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="53795-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="53795-109">**Replyto**が元のメッセージで指定されている場合、インターネットメッセージ形式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに、 **from**の受信者ではなく、 **replyto**の受信者に返信を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="53795-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="53795-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53795-110">Permissions</span></span>
<span data-ttu-id="53795-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53795-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53795-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53795-113">Permission type</span></span>      | <span data-ttu-id="53795-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53795-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53795-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53795-115">Delegated (work or school account)</span></span> | <span data-ttu-id="53795-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53795-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53795-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53795-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53795-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53795-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53795-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53795-119">Application</span></span> | <span data-ttu-id="53795-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53795-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="53795-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53795-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="53795-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53795-122">Request headers</span></span>
| <span data-ttu-id="53795-123">名前</span><span class="sxs-lookup"><span data-stu-id="53795-123">Name</span></span>       | <span data-ttu-id="53795-124">型</span><span class="sxs-lookup"><span data-stu-id="53795-124">Type</span></span> | <span data-ttu-id="53795-125">説明</span><span class="sxs-lookup"><span data-stu-id="53795-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53795-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="53795-126">Authorization</span></span>  | <span data-ttu-id="53795-127">string</span><span class="sxs-lookup"><span data-stu-id="53795-127">string</span></span>  | <span data-ttu-id="53795-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53795-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53795-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53795-130">Content-Type</span></span> | <span data-ttu-id="53795-131">string</span><span class="sxs-lookup"><span data-stu-id="53795-131">string</span></span>  | <span data-ttu-id="53795-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="53795-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53795-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="53795-134">Request body</span></span>
<span data-ttu-id="53795-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="53795-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53795-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="53795-136">Parameter</span></span>    | <span data-ttu-id="53795-137">型</span><span class="sxs-lookup"><span data-stu-id="53795-137">Type</span></span>   |<span data-ttu-id="53795-138">説明</span><span class="sxs-lookup"><span data-stu-id="53795-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53795-139">comment</span><span class="sxs-lookup"><span data-stu-id="53795-139">comment</span></span>|<span data-ttu-id="53795-140">String</span><span class="sxs-lookup"><span data-stu-id="53795-140">String</span></span>|<span data-ttu-id="53795-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="53795-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="53795-143">message</span><span class="sxs-lookup"><span data-stu-id="53795-143">message</span></span>|[<span data-ttu-id="53795-144">message</span><span class="sxs-lookup"><span data-stu-id="53795-144">message</span></span>](../resources/message.md)|<span data-ttu-id="53795-145">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="53795-145">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="53795-146">応答</span><span class="sxs-lookup"><span data-stu-id="53795-146">Response</span></span>

<span data-ttu-id="53795-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53795-147">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53795-148">例</span><span class="sxs-lookup"><span data-stu-id="53795-148">Example</span></span>
<span data-ttu-id="53795-149">次の例では、下書きの返信を作成し、要求の本文にコメントと受信者を追加します。</span><span class="sxs-lookup"><span data-stu-id="53795-149">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="53795-150">要求</span><span class="sxs-lookup"><span data-stu-id="53795-150">Request</span></span>
<span data-ttu-id="53795-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53795-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="53795-152">プロトコル</span><span class="sxs-lookup"><span data-stu-id="53795-152">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="53795-153">C#</span><span class="sxs-lookup"><span data-stu-id="53795-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53795-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="53795-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53795-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="53795-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53795-156">Java</span><span class="sxs-lookup"><span data-stu-id="53795-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53795-157">応答</span><span class="sxs-lookup"><span data-stu-id="53795-157">Response</span></span>
<span data-ttu-id="53795-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53795-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
