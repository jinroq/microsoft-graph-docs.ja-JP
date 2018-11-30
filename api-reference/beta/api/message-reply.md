---
title: 'メッセージ: reply'
description: 'メッセージの送信者に返信やコメントの追加、更新可能なすべて 1 つの**応答**の呼び出しでプロパティを変更します。 '
ms.openlocfilehash: 93130e8a877b9a7bdc553646037f583fd8da84fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071129"
---
# <a name="message-reply"></a><span data-ttu-id="58712-103">メッセージ: reply</span><span class="sxs-lookup"><span data-stu-id="58712-103">message: reply</span></span>

> <span data-ttu-id="58712-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58712-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58712-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58712-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58712-106">メッセージの送信者に返信やコメントの追加、更新可能なすべて 1 つの**応答**の呼び出しでプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="58712-106">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="58712-107">その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="58712-107">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="58712-108">または、最初に[下書きの返信メッセージを作成して](../api/message-createreply.md)コメントを含めるか、メッセージのプロパティを更新し、返信を[送信](../api/message-send.md)します。</span><span class="sxs-lookup"><span data-stu-id="58712-108">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="58712-109">**メモ**</span><span class="sxs-lookup"><span data-stu-id="58712-109">**Note**</span></span>

- <span data-ttu-id="58712-110">**Body**プロパティまたはコメントのいずれかを指定することができます、`message`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="58712-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="58712-111">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="58712-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="58712-112">**ReplyTo**プロパティが元のメッセージのインターネット メッセージ フォーマット ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに指定されている場合は、 **replyTo**で**の**プロパティで受信者ではなく受信者に返信を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="58712-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="58712-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58712-113">Permissions</span></span>
<span data-ttu-id="58712-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58712-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58712-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58712-116">Permission type</span></span>      | <span data-ttu-id="58712-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58712-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58712-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58712-118">Delegated (work or school account)</span></span> | <span data-ttu-id="58712-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="58712-119">Mail.Send</span></span>    |
|<span data-ttu-id="58712-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58712-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58712-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="58712-121">Mail.Send</span></span>    |
|<span data-ttu-id="58712-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58712-122">Application</span></span> | <span data-ttu-id="58712-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="58712-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="58712-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58712-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="58712-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58712-125">Request headers</span></span>
| <span data-ttu-id="58712-126">名前</span><span class="sxs-lookup"><span data-stu-id="58712-126">Name</span></span>       | <span data-ttu-id="58712-127">型</span><span class="sxs-lookup"><span data-stu-id="58712-127">Type</span></span> | <span data-ttu-id="58712-128">説明</span><span class="sxs-lookup"><span data-stu-id="58712-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58712-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="58712-129">Authorization</span></span>  | <span data-ttu-id="58712-130">string</span><span class="sxs-lookup"><span data-stu-id="58712-130">string</span></span>  | <span data-ttu-id="58712-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="58712-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58712-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58712-133">Content-Type</span></span> | <span data-ttu-id="58712-134">string</span><span class="sxs-lookup"><span data-stu-id="58712-134">string</span></span>  | <span data-ttu-id="58712-p106">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="58712-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58712-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="58712-137">Request body</span></span>
<span data-ttu-id="58712-138">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="58712-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58712-139">パラメーター</span><span class="sxs-lookup"><span data-stu-id="58712-139">Parameter</span></span>    | <span data-ttu-id="58712-140">型</span><span class="sxs-lookup"><span data-stu-id="58712-140">Type</span></span>   |<span data-ttu-id="58712-141">説明</span><span class="sxs-lookup"><span data-stu-id="58712-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58712-142">comment</span><span class="sxs-lookup"><span data-stu-id="58712-142">comment</span></span>|<span data-ttu-id="58712-143">String</span><span class="sxs-lookup"><span data-stu-id="58712-143">String</span></span>|<span data-ttu-id="58712-p107">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="58712-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="58712-146">message</span><span class="sxs-lookup"><span data-stu-id="58712-146">message</span></span>|[<span data-ttu-id="58712-147">message</span><span class="sxs-lookup"><span data-stu-id="58712-147">message</span></span>](../resources/message.md)|<span data-ttu-id="58712-148">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="58712-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="58712-149">応答</span><span class="sxs-lookup"><span data-stu-id="58712-149">Response</span></span>

<span data-ttu-id="58712-p108">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="58712-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58712-152">例</span><span class="sxs-lookup"><span data-stu-id="58712-152">Example</span></span>
<span data-ttu-id="58712-153">次の例では、コメントを含め、受信者を返信メッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="58712-153">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="58712-154">要求</span><span class="sxs-lookup"><span data-stu-id="58712-154">Request</span></span>
<span data-ttu-id="58712-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58712-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="58712-156">応答</span><span class="sxs-lookup"><span data-stu-id="58712-156">Response</span></span>
<span data-ttu-id="58712-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="58712-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
