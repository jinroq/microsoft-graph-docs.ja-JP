---
title: 'メッセージ: replyAll'
description: 'コメントを指定して、更新可能なプロパティを変更することにより、メッセージのすべての受信者に返信する '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6bd4df9321a0001d5907b79b8983e9db768f2412
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266515"
---
# <a name="message-replyall"></a><span data-ttu-id="cc9cc-103">メッセージ: replyAll</span><span class="sxs-lookup"><span data-stu-id="cc9cc-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc9cc-104">**ReplyAll**メソッドを使用して、コメントを指定し、返信のために更新可能なプロパティを変更することによって、メッセージのすべての受信者に返信します。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="cc9cc-105">その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="cc9cc-106">または、最初に[下書きの返信メッセージを作成](../api/message-createreplyall.md)してコメントを含めるか、メッセージのプロパティを更新してから、返信を[送信](../api/message-send.md)します。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="cc9cc-107">**注**</span><span class="sxs-lookup"><span data-stu-id="cc9cc-107">**Note**</span></span>

- <span data-ttu-id="cc9cc-108">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="cc9cc-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="cc9cc-109">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="cc9cc-110">元のメッセージで**replyTo**プロパティが指定されている場合、インターネットメッセージ形式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに、受信者に返信を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="cc9cc-111">**replyTo**プロパティ\*\*\*\* と torプロパティのプロパティ。これは、 **from**および**torの piの**各プロパティの受信者ではありません。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="cc9cc-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc9cc-112">Permissions</span></span>
<span data-ttu-id="cc9cc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc9cc-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc9cc-115">Permission type</span></span>      | <span data-ttu-id="cc9cc-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc9cc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc9cc-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc9cc-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cc9cc-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cc9cc-118">Mail.Send</span></span>    |
|<span data-ttu-id="cc9cc-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc9cc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc9cc-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cc9cc-120">Mail.Send</span></span>    |
|<span data-ttu-id="cc9cc-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc9cc-121">Application</span></span> | <span data-ttu-id="cc9cc-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cc9cc-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc9cc-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc9cc-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="cc9cc-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc9cc-124">Request headers</span></span>
| <span data-ttu-id="cc9cc-125">名前</span><span class="sxs-lookup"><span data-stu-id="cc9cc-125">Name</span></span>       | <span data-ttu-id="cc9cc-126">型</span><span class="sxs-lookup"><span data-stu-id="cc9cc-126">Type</span></span> | <span data-ttu-id="cc9cc-127">説明</span><span class="sxs-lookup"><span data-stu-id="cc9cc-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cc9cc-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc9cc-128">Authorization</span></span>  | <span data-ttu-id="cc9cc-129">string</span><span class="sxs-lookup"><span data-stu-id="cc9cc-129">string</span></span>  | <span data-ttu-id="cc9cc-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc9cc-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc9cc-132">Content-Type</span></span> | <span data-ttu-id="cc9cc-133">string</span><span class="sxs-lookup"><span data-stu-id="cc9cc-133">string</span></span>  | <span data-ttu-id="cc9cc-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc9cc-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc9cc-136">Request body</span></span>
<span data-ttu-id="cc9cc-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc9cc-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cc9cc-138">Parameter</span></span>    | <span data-ttu-id="cc9cc-139">型</span><span class="sxs-lookup"><span data-stu-id="cc9cc-139">Type</span></span>   |<span data-ttu-id="cc9cc-140">説明</span><span class="sxs-lookup"><span data-stu-id="cc9cc-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc9cc-141">comment</span><span class="sxs-lookup"><span data-stu-id="cc9cc-141">comment</span></span>|<span data-ttu-id="cc9cc-142">String</span><span class="sxs-lookup"><span data-stu-id="cc9cc-142">String</span></span>|<span data-ttu-id="cc9cc-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="cc9cc-145">message</span><span class="sxs-lookup"><span data-stu-id="cc9cc-145">message</span></span>|[<span data-ttu-id="cc9cc-146">message</span><span class="sxs-lookup"><span data-stu-id="cc9cc-146">message</span></span>](../resources/message.md)|<span data-ttu-id="cc9cc-147">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="cc9cc-148">応答</span><span class="sxs-lookup"><span data-stu-id="cc9cc-148">Response</span></span>

<span data-ttu-id="cc9cc-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc9cc-151">例</span><span class="sxs-lookup"><span data-stu-id="cc9cc-151">Example</span></span>
<span data-ttu-id="cc9cc-152">次の例では、コメントを含め、添付ファイルを全員に返信メッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="cc9cc-153">要求</span><span class="sxs-lookup"><span data-stu-id="cc9cc-153">Request</span></span>
<span data-ttu-id="cc9cc-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-154">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="cc9cc-155">応答</span><span class="sxs-lookup"><span data-stu-id="cc9cc-155">Response</span></span>
<span data-ttu-id="cc9cc-156">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cc9cc-156">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cc9cc-157">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="cc9cc-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cc9cc-158">C#</span><span class="sxs-lookup"><span data-stu-id="cc9cc-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_replyall-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc9cc-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc9cc-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_replyall-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cc9cc-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="cc9cc-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_replyall-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
