---
title: 'メッセージ: createForward'
description: 'コメントを含めるまたはメッセージ プロパティを更新するメッセージを転送の下書きを作成します。  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 56f73ac798ef3440b66cb4c0de1192d3248d3a61
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949074"
---
# <a name="message-createforward"></a><span data-ttu-id="ff009-103">メッセージ: createForward</span><span class="sxs-lookup"><span data-stu-id="ff009-103">message: createForward</span></span>

> <span data-ttu-id="ff009-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff009-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff009-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff009-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff009-106">コメントを含めるまたはメッセージ プロパティを更新するメッセージを転送の下書きを作成します。</span><span class="sxs-lookup"><span data-stu-id="ff009-106">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="ff009-107">すべてで 1 つの**createForward**を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="ff009-107">all in one **createForward** call.</span></span> <span data-ttu-id="ff009-108">[下書きメッセージ[を送信](../api/message-send.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="ff009-108">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="ff009-109">**注**</span><span class="sxs-lookup"><span data-stu-id="ff009-109">**Note**</span></span>

- <span data-ttu-id="ff009-110">**Body**プロパティまたはコメントのいずれかを指定することができます、`message`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="ff009-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="ff009-111">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff009-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="ff009-112">どちらかを指定する必要があります、`toRecipients`の**toRecipients**プロパティは、パラメーター、または、`message`パラメーター。</span><span class="sxs-lookup"><span data-stu-id="ff009-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="ff009-113">両方を指定するか、どちらも指定しないと、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff009-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff009-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff009-114">Permissions</span></span>
<span data-ttu-id="ff009-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff009-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff009-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff009-117">Permission type</span></span>      | <span data-ttu-id="ff009-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff009-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff009-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff009-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ff009-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff009-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ff009-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff009-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff009-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff009-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ff009-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff009-123">Application</span></span> | <span data-ttu-id="ff009-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff009-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff009-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff009-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="ff009-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff009-126">Request headers</span></span>
| <span data-ttu-id="ff009-127">名前</span><span class="sxs-lookup"><span data-stu-id="ff009-127">Name</span></span>       | <span data-ttu-id="ff009-128">種類</span><span class="sxs-lookup"><span data-stu-id="ff009-128">Type</span></span> | <span data-ttu-id="ff009-129">説明</span><span class="sxs-lookup"><span data-stu-id="ff009-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff009-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff009-130">Authorization</span></span>  | <span data-ttu-id="ff009-131">string</span><span class="sxs-lookup"><span data-stu-id="ff009-131">string</span></span>  | <span data-ttu-id="ff009-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff009-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff009-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff009-134">Content-Type</span></span> | <span data-ttu-id="ff009-135">string</span><span class="sxs-lookup"><span data-stu-id="ff009-135">string</span></span>  | <span data-ttu-id="ff009-p107">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="ff009-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff009-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff009-138">Request body</span></span>
<span data-ttu-id="ff009-139">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ff009-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ff009-140">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff009-140">Parameter</span></span>    | <span data-ttu-id="ff009-141">Type</span><span class="sxs-lookup"><span data-stu-id="ff009-141">Type</span></span>   |<span data-ttu-id="ff009-142">説明</span><span class="sxs-lookup"><span data-stu-id="ff009-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff009-143">comment</span><span class="sxs-lookup"><span data-stu-id="ff009-143">comment</span></span>|<span data-ttu-id="ff009-144">String</span><span class="sxs-lookup"><span data-stu-id="ff009-144">String</span></span>|<span data-ttu-id="ff009-p108">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ff009-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ff009-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="ff009-147">toRecipients</span></span>|<span data-ttu-id="ff009-148">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="ff009-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="ff009-149">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="ff009-149">The list of recipients.</span></span>|
|<span data-ttu-id="ff009-150">message</span><span class="sxs-lookup"><span data-stu-id="ff009-150">message</span></span>|[<span data-ttu-id="ff009-151">message</span><span class="sxs-lookup"><span data-stu-id="ff009-151">message</span></span>](../resources/message.md)|<span data-ttu-id="ff009-152">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="ff009-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="ff009-153">応答</span><span class="sxs-lookup"><span data-stu-id="ff009-153">Response</span></span>

<span data-ttu-id="ff009-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff009-154">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff009-155">例</span><span class="sxs-lookup"><span data-stu-id="ff009-155">Example</span></span>
<span data-ttu-id="ff009-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ff009-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff009-157">要求</span><span class="sxs-lookup"><span data-stu-id="ff009-157">Request</span></span>
<span data-ttu-id="ff009-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff009-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```

##### <a name="response"></a><span data-ttu-id="ff009-159">応答</span><span class="sxs-lookup"><span data-stu-id="ff009-159">Response</span></span>
<span data-ttu-id="ff009-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff009-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
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
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
