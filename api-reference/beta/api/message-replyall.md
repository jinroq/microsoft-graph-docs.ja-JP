---
title: 'メッセージ: replyAll'
description: 'コメントを指定して、更新可能なプロパティを変更することによって、メッセージの受信者全員に返信します。 '
ms.openlocfilehash: c79320229aad67a406a6519762c7cdd99af2ad50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072957"
---
# <a name="message-replyall"></a><span data-ttu-id="33d80-103">メッセージ: replyAll</span><span class="sxs-lookup"><span data-stu-id="33d80-103">message: replyAll</span></span>

> <span data-ttu-id="33d80-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33d80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33d80-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33d80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33d80-106">コメントを指定して、 **replyAll**メソッドを使用して、すべての返信、更新可能なプロパティを変更することによって、メッセージの受信者全員に返信します。</span><span class="sxs-lookup"><span data-stu-id="33d80-106">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="33d80-107">その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="33d80-107">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="33d80-108">または、最初の[ドラフトの全員に返信メッセージを作成する](../api/message-createreplyall.md)コメントを含めるか、メッセージのプロパティ、および更新し、返信[を送信](../api/message-send.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="33d80-108">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="33d80-109">**メモ**</span><span class="sxs-lookup"><span data-stu-id="33d80-109">**Note**</span></span>

- <span data-ttu-id="33d80-110">**Body**プロパティまたはコメントのいずれかを指定することができます、`message`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="33d80-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="33d80-111">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="33d80-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="33d80-112">**ReplyTo**プロパティが元のメッセージのインターネット メッセージ フォーマット ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに指定されている場合は、内の受信者に返信を送信する必要があります、</span><span class="sxs-lookup"><span data-stu-id="33d80-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="33d80-113">**replyTo**と**toRecipients**プロパティと**から**と**toRecipients**プロパティで受信者ではありません。</span><span class="sxs-lookup"><span data-stu-id="33d80-113">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="33d80-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33d80-114">Permissions</span></span>
<span data-ttu-id="33d80-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33d80-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33d80-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33d80-117">Permission type</span></span>      | <span data-ttu-id="33d80-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="33d80-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33d80-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33d80-119">Delegated (work or school account)</span></span> | <span data-ttu-id="33d80-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="33d80-120">Mail.Send</span></span>    |
|<span data-ttu-id="33d80-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33d80-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33d80-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="33d80-122">Mail.Send</span></span>    |
|<span data-ttu-id="33d80-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33d80-123">Application</span></span> | <span data-ttu-id="33d80-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="33d80-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="33d80-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33d80-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="33d80-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33d80-126">Request headers</span></span>
| <span data-ttu-id="33d80-127">名前</span><span class="sxs-lookup"><span data-stu-id="33d80-127">Name</span></span>       | <span data-ttu-id="33d80-128">型</span><span class="sxs-lookup"><span data-stu-id="33d80-128">Type</span></span> | <span data-ttu-id="33d80-129">説明</span><span class="sxs-lookup"><span data-stu-id="33d80-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33d80-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="33d80-130">Authorization</span></span>  | <span data-ttu-id="33d80-131">string</span><span class="sxs-lookup"><span data-stu-id="33d80-131">string</span></span>  | <span data-ttu-id="33d80-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33d80-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33d80-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33d80-134">Content-Type</span></span> | <span data-ttu-id="33d80-135">string</span><span class="sxs-lookup"><span data-stu-id="33d80-135">string</span></span>  | <span data-ttu-id="33d80-p106">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="33d80-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33d80-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="33d80-138">Request body</span></span>
<span data-ttu-id="33d80-139">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="33d80-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33d80-140">パラメーター</span><span class="sxs-lookup"><span data-stu-id="33d80-140">Parameter</span></span>    | <span data-ttu-id="33d80-141">型</span><span class="sxs-lookup"><span data-stu-id="33d80-141">Type</span></span>   |<span data-ttu-id="33d80-142">説明</span><span class="sxs-lookup"><span data-stu-id="33d80-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33d80-143">comment</span><span class="sxs-lookup"><span data-stu-id="33d80-143">comment</span></span>|<span data-ttu-id="33d80-144">String</span><span class="sxs-lookup"><span data-stu-id="33d80-144">String</span></span>|<span data-ttu-id="33d80-p107">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="33d80-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="33d80-147">message</span><span class="sxs-lookup"><span data-stu-id="33d80-147">message</span></span>|[<span data-ttu-id="33d80-148">message</span><span class="sxs-lookup"><span data-stu-id="33d80-148">message</span></span>](../resources/message.md)|<span data-ttu-id="33d80-149">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="33d80-149">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="33d80-150">応答</span><span class="sxs-lookup"><span data-stu-id="33d80-150">Response</span></span>

<span data-ttu-id="33d80-p108">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="33d80-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33d80-153">例</span><span class="sxs-lookup"><span data-stu-id="33d80-153">Example</span></span>
<span data-ttu-id="33d80-154">次の例では、コメントを含め、添付ファイルを全員に返信メッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="33d80-154">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="33d80-155">要求</span><span class="sxs-lookup"><span data-stu-id="33d80-155">Request</span></span>
<span data-ttu-id="33d80-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33d80-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
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
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```


##### <a name="response"></a><span data-ttu-id="33d80-157">応答</span><span class="sxs-lookup"><span data-stu-id="33d80-157">Response</span></span>
<span data-ttu-id="33d80-158">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="33d80-158">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
