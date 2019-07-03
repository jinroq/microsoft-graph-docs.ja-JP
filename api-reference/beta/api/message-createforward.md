---
title: 'メッセージ: createForward'
description: '下書きの転送メッセージを作成してコメントを含めるか、メッセージのプロパティを更新します。  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0b1ce182e58d5e2033b1e9cac0f1025df1dd6e89
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448279"
---
# <a name="message-createforward"></a><span data-ttu-id="1511f-103">メッセージ: createForward</span><span class="sxs-lookup"><span data-stu-id="1511f-103">message: createForward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1511f-104">下書きの転送メッセージを作成してコメントを含めるか、メッセージのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1511f-104">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="1511f-105">1つの**Createforward**呼び出し内のすべて。</span><span class="sxs-lookup"><span data-stu-id="1511f-105">all in one **createForward** call.</span></span> <span data-ttu-id="1511f-106">その後、下書きメッセージを[送信](../api/message-send.md)できます。</span><span class="sxs-lookup"><span data-stu-id="1511f-106">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="1511f-107">**注**</span><span class="sxs-lookup"><span data-stu-id="1511f-107">**Note**</span></span>

- <span data-ttu-id="1511f-108">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="1511f-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="1511f-109">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="1511f-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="1511f-110">パラメーターを指定するか`toRecipients` 、 `message`パラメーターの**トーラス**プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1511f-110">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="1511f-111">両方を指定するか、どちらも指定しないと、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="1511f-111">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="1511f-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1511f-112">Permissions</span></span>
<span data-ttu-id="1511f-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1511f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1511f-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1511f-115">Permission type</span></span>      | <span data-ttu-id="1511f-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1511f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1511f-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1511f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1511f-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1511f-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1511f-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1511f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1511f-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1511f-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1511f-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1511f-121">Application</span></span> | <span data-ttu-id="1511f-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1511f-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1511f-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1511f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="1511f-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1511f-124">Request headers</span></span>
| <span data-ttu-id="1511f-125">名前</span><span class="sxs-lookup"><span data-stu-id="1511f-125">Name</span></span>       | <span data-ttu-id="1511f-126">型</span><span class="sxs-lookup"><span data-stu-id="1511f-126">Type</span></span> | <span data-ttu-id="1511f-127">説明</span><span class="sxs-lookup"><span data-stu-id="1511f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1511f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1511f-128">Authorization</span></span>  | <span data-ttu-id="1511f-129">string</span><span class="sxs-lookup"><span data-stu-id="1511f-129">string</span></span>  | <span data-ttu-id="1511f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1511f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1511f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1511f-132">Content-Type</span></span> | <span data-ttu-id="1511f-133">string</span><span class="sxs-lookup"><span data-stu-id="1511f-133">string</span></span>  | <span data-ttu-id="1511f-p106">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="1511f-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1511f-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="1511f-136">Request body</span></span>
<span data-ttu-id="1511f-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1511f-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1511f-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1511f-138">Parameter</span></span>    | <span data-ttu-id="1511f-139">型</span><span class="sxs-lookup"><span data-stu-id="1511f-139">Type</span></span>   |<span data-ttu-id="1511f-140">説明</span><span class="sxs-lookup"><span data-stu-id="1511f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1511f-141">comment</span><span class="sxs-lookup"><span data-stu-id="1511f-141">comment</span></span>|<span data-ttu-id="1511f-142">String</span><span class="sxs-lookup"><span data-stu-id="1511f-142">String</span></span>|<span data-ttu-id="1511f-p107">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1511f-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="1511f-145">toRecipients</span><span class="sxs-lookup"><span data-stu-id="1511f-145">toRecipients</span></span>|<span data-ttu-id="1511f-146">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="1511f-146">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="1511f-147">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="1511f-147">The list of recipients.</span></span>|
|<span data-ttu-id="1511f-148">message</span><span class="sxs-lookup"><span data-stu-id="1511f-148">message</span></span>|[<span data-ttu-id="1511f-149">message</span><span class="sxs-lookup"><span data-stu-id="1511f-149">message</span></span>](../resources/message.md)|<span data-ttu-id="1511f-150">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="1511f-150">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="1511f-151">応答</span><span class="sxs-lookup"><span data-stu-id="1511f-151">Response</span></span>

<span data-ttu-id="1511f-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1511f-152">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1511f-153">例</span><span class="sxs-lookup"><span data-stu-id="1511f-153">Example</span></span>
<span data-ttu-id="1511f-154">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1511f-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1511f-155">要求</span><span class="sxs-lookup"><span data-stu-id="1511f-155">Request</span></span>
<span data-ttu-id="1511f-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1511f-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1511f-157">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1511f-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1511f-158">C#</span><span class="sxs-lookup"><span data-stu-id="1511f-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1511f-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="1511f-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1511f-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="1511f-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1511f-161">応答</span><span class="sxs-lookup"><span data-stu-id="1511f-161">Response</span></span>
<span data-ttu-id="1511f-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1511f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
  ]
}
-->
