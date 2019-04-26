---
title: 'メッセージ: createForward'
description: '下書きの転送メッセージを作成してコメントを含めるか、メッセージのプロパティを更新します。  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d863c582a704edd095b69dc5442cac8ce74f9613
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333171"
---
# <a name="message-createforward"></a><span data-ttu-id="84fb1-103">メッセージ: createForward</span><span class="sxs-lookup"><span data-stu-id="84fb1-103">message: createForward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84fb1-104">下書きの転送メッセージを作成してコメントを含めるか、メッセージのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="84fb1-104">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="84fb1-105">1つの**createforward**呼び出し内のすべて。</span><span class="sxs-lookup"><span data-stu-id="84fb1-105">all in one **createForward** call.</span></span> <span data-ttu-id="84fb1-106">その後、下書きメッセージを[送信](../api/message-send.md)できます。</span><span class="sxs-lookup"><span data-stu-id="84fb1-106">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="84fb1-107">**注**</span><span class="sxs-lookup"><span data-stu-id="84fb1-107">**Note**</span></span>

- <span data-ttu-id="84fb1-108">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="84fb1-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="84fb1-109">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="84fb1-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="84fb1-110">パラメーターを指定するか`toRecipients` 、 `message`パラメーターの**トーラス**プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="84fb1-110">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="84fb1-111">両方を指定するか、どちらも指定しないと、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="84fb1-111">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="84fb1-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84fb1-112">Permissions</span></span>
<span data-ttu-id="84fb1-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84fb1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84fb1-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84fb1-115">Permission type</span></span>      | <span data-ttu-id="84fb1-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84fb1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84fb1-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84fb1-117">Delegated (work or school account)</span></span> | <span data-ttu-id="84fb1-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84fb1-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="84fb1-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84fb1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84fb1-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84fb1-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="84fb1-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84fb1-121">Application</span></span> | <span data-ttu-id="84fb1-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84fb1-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="84fb1-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84fb1-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="84fb1-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84fb1-124">Request headers</span></span>
| <span data-ttu-id="84fb1-125">名前</span><span class="sxs-lookup"><span data-stu-id="84fb1-125">Name</span></span>       | <span data-ttu-id="84fb1-126">型</span><span class="sxs-lookup"><span data-stu-id="84fb1-126">Type</span></span> | <span data-ttu-id="84fb1-127">説明</span><span class="sxs-lookup"><span data-stu-id="84fb1-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="84fb1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="84fb1-128">Authorization</span></span>  | <span data-ttu-id="84fb1-129">string</span><span class="sxs-lookup"><span data-stu-id="84fb1-129">string</span></span>  | <span data-ttu-id="84fb1-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="84fb1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84fb1-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84fb1-132">Content-Type</span></span> | <span data-ttu-id="84fb1-133">string</span><span class="sxs-lookup"><span data-stu-id="84fb1-133">string</span></span>  | <span data-ttu-id="84fb1-p106">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="84fb1-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84fb1-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="84fb1-136">Request body</span></span>
<span data-ttu-id="84fb1-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="84fb1-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="84fb1-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="84fb1-138">Parameter</span></span>    | <span data-ttu-id="84fb1-139">型</span><span class="sxs-lookup"><span data-stu-id="84fb1-139">Type</span></span>   |<span data-ttu-id="84fb1-140">説明</span><span class="sxs-lookup"><span data-stu-id="84fb1-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84fb1-141">comment</span><span class="sxs-lookup"><span data-stu-id="84fb1-141">comment</span></span>|<span data-ttu-id="84fb1-142">String</span><span class="sxs-lookup"><span data-stu-id="84fb1-142">String</span></span>|<span data-ttu-id="84fb1-p107">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="84fb1-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="84fb1-145">toRecipients</span><span class="sxs-lookup"><span data-stu-id="84fb1-145">toRecipients</span></span>|<span data-ttu-id="84fb1-146">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="84fb1-146">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="84fb1-147">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="84fb1-147">The list of recipients.</span></span>|
|<span data-ttu-id="84fb1-148">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="84fb1-148">message</span></span>|[<span data-ttu-id="84fb1-149">message</span><span class="sxs-lookup"><span data-stu-id="84fb1-149">message</span></span>](../resources/message.md)|<span data-ttu-id="84fb1-150">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="84fb1-150">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="84fb1-151">応答</span><span class="sxs-lookup"><span data-stu-id="84fb1-151">Response</span></span>

<span data-ttu-id="84fb1-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="84fb1-152">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84fb1-153">例</span><span class="sxs-lookup"><span data-stu-id="84fb1-153">Example</span></span>
<span data-ttu-id="84fb1-154">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="84fb1-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="84fb1-155">要求</span><span class="sxs-lookup"><span data-stu-id="84fb1-155">Request</span></span>
<span data-ttu-id="84fb1-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="84fb1-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="84fb1-157">応答</span><span class="sxs-lookup"><span data-stu-id="84fb1-157">Response</span></span>
<span data-ttu-id="84fb1-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="84fb1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
