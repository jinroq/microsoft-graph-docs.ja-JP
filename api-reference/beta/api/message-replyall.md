---
title: 'メッセージ: replyAll'
description: 'コメントを指定して、更新可能なプロパティを変更することによって、メッセージの受信者全員に返信します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 05f552676400196aed275c32020bcdf5211d0e31
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528614"
---
# <a name="message-replyall"></a><span data-ttu-id="0c69e-103">メッセージ: replyAll</span><span class="sxs-lookup"><span data-stu-id="0c69e-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c69e-p101">コメントを指定して、**更新可能なプロパティ**を変更することによってメッセージ受信者全員に返信し、全員に ReplyAll メソッドを使用します。その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="0c69e-p101">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="0c69e-106">または、最初の[ドラフトの全員に返信メッセージを作成する](../api/message-createreplyall.md)コメントを含めるか、メッセージのプロパティ、および更新し、返信[を送信](../api/message-send.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="0c69e-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="0c69e-107">**注**</span><span class="sxs-lookup"><span data-stu-id="0c69e-107">**Note**</span></span>

- <span data-ttu-id="0c69e-p102">コメントまたは `message` パラメーターの **Body** プロパティを指定できます。両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="0c69e-p102">You can specify either a comment or the **body** property of the `message` parameter. Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="0c69e-110">**ReplyTo**プロパティが元のメッセージのインターネット メッセージ フォーマット ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) ごとに指定されている場合は、内の受信者に返信を送信する必要があります、</span><span class="sxs-lookup"><span data-stu-id="0c69e-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="0c69e-111">**replyTo**と**toRecipients**プロパティと**から**と**toRecipients**プロパティで受信者ではありません。</span><span class="sxs-lookup"><span data-stu-id="0c69e-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0c69e-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c69e-112">Permissions</span></span>
<span data-ttu-id="0c69e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c69e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c69e-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c69e-115">Permission type</span></span>      | <span data-ttu-id="0c69e-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c69e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c69e-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c69e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0c69e-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0c69e-118">Mail.Send</span></span>    |
|<span data-ttu-id="0c69e-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c69e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c69e-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0c69e-120">Mail.Send</span></span>    |
|<span data-ttu-id="0c69e-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c69e-121">Application</span></span> | <span data-ttu-id="0c69e-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0c69e-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c69e-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c69e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="0c69e-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c69e-124">Request headers</span></span>
| <span data-ttu-id="0c69e-125">名前</span><span class="sxs-lookup"><span data-stu-id="0c69e-125">Name</span></span>       | <span data-ttu-id="0c69e-126">型</span><span class="sxs-lookup"><span data-stu-id="0c69e-126">Type</span></span> | <span data-ttu-id="0c69e-127">説明</span><span class="sxs-lookup"><span data-stu-id="0c69e-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c69e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c69e-128">Authorization</span></span>  | <span data-ttu-id="0c69e-129">string</span><span class="sxs-lookup"><span data-stu-id="0c69e-129">string</span></span>  | <span data-ttu-id="0c69e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0c69e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c69e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c69e-132">Content-Type</span></span> | <span data-ttu-id="0c69e-133">string</span><span class="sxs-lookup"><span data-stu-id="0c69e-133">string</span></span>  | <span data-ttu-id="0c69e-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="0c69e-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c69e-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c69e-136">Request body</span></span>
<span data-ttu-id="0c69e-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0c69e-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c69e-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c69e-138">Parameter</span></span>    | <span data-ttu-id="0c69e-139">型</span><span class="sxs-lookup"><span data-stu-id="0c69e-139">Type</span></span>   |<span data-ttu-id="0c69e-140">説明</span><span class="sxs-lookup"><span data-stu-id="0c69e-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c69e-141">comment</span><span class="sxs-lookup"><span data-stu-id="0c69e-141">comment</span></span>|<span data-ttu-id="0c69e-142">String</span><span class="sxs-lookup"><span data-stu-id="0c69e-142">String</span></span>|<span data-ttu-id="0c69e-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0c69e-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="0c69e-145">message</span><span class="sxs-lookup"><span data-stu-id="0c69e-145">message</span></span>|[<span data-ttu-id="0c69e-146">message</span><span class="sxs-lookup"><span data-stu-id="0c69e-146">message</span></span>](../resources/message.md)|<span data-ttu-id="0c69e-147">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="0c69e-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="0c69e-148">応答</span><span class="sxs-lookup"><span data-stu-id="0c69e-148">Response</span></span>

<span data-ttu-id="0c69e-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0c69e-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c69e-151">例</span><span class="sxs-lookup"><span data-stu-id="0c69e-151">Example</span></span>
<span data-ttu-id="0c69e-152">次の例では、コメントを含め、添付ファイルを全員に返信メッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="0c69e-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="0c69e-153">要求</span><span class="sxs-lookup"><span data-stu-id="0c69e-153">Request</span></span>
<span data-ttu-id="0c69e-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c69e-154">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="0c69e-155">応答</span><span class="sxs-lookup"><span data-stu-id="0c69e-155">Response</span></span>
<span data-ttu-id="0c69e-156">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0c69e-156">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
