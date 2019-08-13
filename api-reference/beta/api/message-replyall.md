---
title: 'メッセージ: replyAll'
description: 'コメントを指定して、更新可能なプロパティを変更することにより、メッセージのすべての受信者に返信する '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b49e4ac2b2d88ac7d5841f3adb39c5ce6efafba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342818"
---
# <a name="message-replyall"></a><span data-ttu-id="d08d2-103">メッセージ: replyAll</span><span class="sxs-lookup"><span data-stu-id="d08d2-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d08d2-104">**ReplyAll**メソッドを使用して、コメントを指定し、返信のために更新可能なプロパティを変更することによって、メッセージのすべての受信者に返信します。</span><span class="sxs-lookup"><span data-stu-id="d08d2-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="d08d2-105">その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="d08d2-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="d08d2-106">または、最初に[下書きの返信メッセージを作成](../api/message-createreplyall.md)してコメントを含めるか、メッセージのプロパティを更新してから、返信を[送信](../api/message-send.md)します。</span><span class="sxs-lookup"><span data-stu-id="d08d2-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="d08d2-107">**注**</span><span class="sxs-lookup"><span data-stu-id="d08d2-107">**Note**</span></span>

- <span data-ttu-id="d08d2-108">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="d08d2-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="d08d2-109">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="d08d2-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="d08d2-110">元のメッセージで**replyTo**プロパティが指定されている場合、インターネットメッセージ形式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに、受信者に返信を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d08d2-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="d08d2-111">**replyTo**プロパティ\*\*\*\* と torプロパティのプロパティ。これは、 **from**および**torの piの**各プロパティの受信者ではありません。</span><span class="sxs-lookup"><span data-stu-id="d08d2-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d08d2-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d08d2-112">Permissions</span></span>
<span data-ttu-id="d08d2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d08d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d08d2-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d08d2-115">Permission type</span></span>      | <span data-ttu-id="d08d2-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d08d2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d08d2-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d08d2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="d08d2-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d08d2-118">Mail.Send</span></span>    |
|<span data-ttu-id="d08d2-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d08d2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d08d2-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d08d2-120">Mail.Send</span></span>    |
|<span data-ttu-id="d08d2-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d08d2-121">Application</span></span> | <span data-ttu-id="d08d2-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d08d2-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d08d2-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d08d2-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="d08d2-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d08d2-124">Request headers</span></span>
| <span data-ttu-id="d08d2-125">名前</span><span class="sxs-lookup"><span data-stu-id="d08d2-125">Name</span></span>       | <span data-ttu-id="d08d2-126">型</span><span class="sxs-lookup"><span data-stu-id="d08d2-126">Type</span></span> | <span data-ttu-id="d08d2-127">説明</span><span class="sxs-lookup"><span data-stu-id="d08d2-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d08d2-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d08d2-128">Authorization</span></span>  | <span data-ttu-id="d08d2-129">string</span><span class="sxs-lookup"><span data-stu-id="d08d2-129">string</span></span>  | <span data-ttu-id="d08d2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d08d2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d08d2-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d08d2-132">Content-Type</span></span> | <span data-ttu-id="d08d2-133">string</span><span class="sxs-lookup"><span data-stu-id="d08d2-133">string</span></span>  | <span data-ttu-id="d08d2-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="d08d2-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d08d2-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="d08d2-136">Request body</span></span>
<span data-ttu-id="d08d2-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d08d2-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d08d2-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d08d2-138">Parameter</span></span>    | <span data-ttu-id="d08d2-139">型</span><span class="sxs-lookup"><span data-stu-id="d08d2-139">Type</span></span>   |<span data-ttu-id="d08d2-140">説明</span><span class="sxs-lookup"><span data-stu-id="d08d2-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d08d2-141">comment</span><span class="sxs-lookup"><span data-stu-id="d08d2-141">comment</span></span>|<span data-ttu-id="d08d2-142">String</span><span class="sxs-lookup"><span data-stu-id="d08d2-142">String</span></span>|<span data-ttu-id="d08d2-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d08d2-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="d08d2-145">message</span><span class="sxs-lookup"><span data-stu-id="d08d2-145">message</span></span>|[<span data-ttu-id="d08d2-146">message</span><span class="sxs-lookup"><span data-stu-id="d08d2-146">message</span></span>](../resources/message.md)|<span data-ttu-id="d08d2-147">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="d08d2-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="d08d2-148">応答</span><span class="sxs-lookup"><span data-stu-id="d08d2-148">Response</span></span>

<span data-ttu-id="d08d2-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d08d2-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d08d2-151">例</span><span class="sxs-lookup"><span data-stu-id="d08d2-151">Example</span></span>
<span data-ttu-id="d08d2-152">次の例では、コメントを含め、添付ファイルを全員に返信メッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="d08d2-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="d08d2-153">要求</span><span class="sxs-lookup"><span data-stu-id="d08d2-153">Request</span></span>
<span data-ttu-id="d08d2-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d08d2-154">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d08d2-155">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d08d2-155">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d08d2-156">C#</span><span class="sxs-lookup"><span data-stu-id="d08d2-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d08d2-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d08d2-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d08d2-158">目的-C</span><span class="sxs-lookup"><span data-stu-id="d08d2-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d08d2-159">Java</span><span class="sxs-lookup"><span data-stu-id="d08d2-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="d08d2-160">応答</span><span class="sxs-lookup"><span data-stu-id="d08d2-160">Response</span></span>
<span data-ttu-id="d08d2-161">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d08d2-161">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
