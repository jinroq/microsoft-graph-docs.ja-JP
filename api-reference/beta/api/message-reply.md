---
title: 'メッセージ: reply'
description: '1 回の **reply** 呼び出しでメッセージ送信者に返信、コメントを追加、または更新可能なプロパティを変更します。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2c79861fbb452ac593d8a97d6c78a6a70d435631
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415002"
---
# <a name="message-reply"></a><span data-ttu-id="ae8aa-103">メッセージ: reply</span><span class="sxs-lookup"><span data-stu-id="ae8aa-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae8aa-p101">1 回の reply 呼び出しでメッセージ送信者に返信、コメントを追加、または更新可能なプロパティを変更します。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-p101">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="ae8aa-106">または、最初に[下書きの返信メッセージを作成して](../api/message-createreply.md)コメントを含めるか、メッセージのプロパティを更新し、返信を[送信](../api/message-send.md)します。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="ae8aa-107">**注**</span><span class="sxs-lookup"><span data-stu-id="ae8aa-107">**Note**</span></span>

- <span data-ttu-id="ae8aa-108">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="ae8aa-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="ae8aa-109">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="ae8aa-110">元のメッセージで**replyto**プロパティが指定されている場合、インターネットメッセージ形式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに、 **from**プロパティで受信者ではなく、 **replyto**の受信者に返信を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="ae8aa-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae8aa-111">Permissions</span></span>
<span data-ttu-id="ae8aa-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae8aa-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae8aa-114">Permission type</span></span>      | <span data-ttu-id="ae8aa-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae8aa-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae8aa-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae8aa-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ae8aa-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ae8aa-117">Mail.Send</span></span>    |
|<span data-ttu-id="ae8aa-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae8aa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae8aa-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ae8aa-119">Mail.Send</span></span>    |
|<span data-ttu-id="ae8aa-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae8aa-120">Application</span></span> | <span data-ttu-id="ae8aa-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ae8aa-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae8aa-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae8aa-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="ae8aa-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae8aa-123">Request headers</span></span>
| <span data-ttu-id="ae8aa-124">名前</span><span class="sxs-lookup"><span data-stu-id="ae8aa-124">Name</span></span>       | <span data-ttu-id="ae8aa-125">型</span><span class="sxs-lookup"><span data-stu-id="ae8aa-125">Type</span></span> | <span data-ttu-id="ae8aa-126">説明</span><span class="sxs-lookup"><span data-stu-id="ae8aa-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ae8aa-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae8aa-127">Authorization</span></span>  | <span data-ttu-id="ae8aa-128">string</span><span class="sxs-lookup"><span data-stu-id="ae8aa-128">string</span></span>  | <span data-ttu-id="ae8aa-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae8aa-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae8aa-131">Content-Type</span></span> | <span data-ttu-id="ae8aa-132">string</span><span class="sxs-lookup"><span data-stu-id="ae8aa-132">string</span></span>  | <span data-ttu-id="ae8aa-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae8aa-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae8aa-135">Request body</span></span>
<span data-ttu-id="ae8aa-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae8aa-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae8aa-137">Parameter</span></span>    | <span data-ttu-id="ae8aa-138">型</span><span class="sxs-lookup"><span data-stu-id="ae8aa-138">Type</span></span>   |<span data-ttu-id="ae8aa-139">説明</span><span class="sxs-lookup"><span data-stu-id="ae8aa-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae8aa-140">comment</span><span class="sxs-lookup"><span data-stu-id="ae8aa-140">comment</span></span>|<span data-ttu-id="ae8aa-141">String</span><span class="sxs-lookup"><span data-stu-id="ae8aa-141">String</span></span>|<span data-ttu-id="ae8aa-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ae8aa-144">message</span><span class="sxs-lookup"><span data-stu-id="ae8aa-144">message</span></span>|[<span data-ttu-id="ae8aa-145">message</span><span class="sxs-lookup"><span data-stu-id="ae8aa-145">message</span></span>](../resources/message.md)|<span data-ttu-id="ae8aa-146">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="ae8aa-147">応答</span><span class="sxs-lookup"><span data-stu-id="ae8aa-147">Response</span></span>

<span data-ttu-id="ae8aa-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae8aa-150">例</span><span class="sxs-lookup"><span data-stu-id="ae8aa-150">Example</span></span>
<span data-ttu-id="ae8aa-151">次の例では、コメントを含め、受信者を返信メッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="ae8aa-152">要求</span><span class="sxs-lookup"><span data-stu-id="ae8aa-152">Request</span></span>
<span data-ttu-id="ae8aa-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-153">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ae8aa-154">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ae8aa-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
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
  "comment": "Samantha, Randi, would you name the group please?" 
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ae8aa-155">C#</span><span class="sxs-lookup"><span data-stu-id="ae8aa-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae8aa-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae8aa-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae8aa-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="ae8aa-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ae8aa-158">応答</span><span class="sxs-lookup"><span data-stu-id="ae8aa-158">Response</span></span>
<span data-ttu-id="ae8aa-159">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ae8aa-159">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
