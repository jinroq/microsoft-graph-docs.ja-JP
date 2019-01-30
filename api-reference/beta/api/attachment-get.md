---
title: 添付ファイルを取得する
description: プロパティとイベント、メッセージ、Outlook のタスク、または投稿に添付された添付ファイルの関係を参照してください。
localization_priority: Normal
ms.openlocfilehash: b346461dad8b0a15d12d0882e0fe8aa4cc2d4774
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641163"
---
# <a name="get-attachment"></a><span data-ttu-id="4f7f5-103">添付ファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="4f7f5-103">Get attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f7f5-104">プロパティと[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付された添付ファイルの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

<span data-ttu-id="4f7f5-105">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="4f7f5-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="4f7f5-p101">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)。`$expand` を使用すると、その項目のプロパティをさらに取得できます。次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-p101">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource). You can use `$expand` to further get the properties of that item. See an [example](#request-2) below.</span></span>
* <span data-ttu-id="4f7f5-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="4f7f5-111">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f7f5-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f7f5-112">Permissions</span></span>

<span data-ttu-id="4f7f5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="4f7f5-115">メッセージの添付ファイルにアクセスする場合: Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4f7f5-115">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="4f7f5-116">イベントで添付ファイルにアクセスする場合: Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4f7f5-116">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="4f7f5-117">Outlook からのタスクの添付ファイルにアクセスする場合: Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="4f7f5-117">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="4f7f5-118">グループの投稿の添付ファイルにアクセスする場合: Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f7f5-118">If accessing attachments in group posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="4f7f5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f7f5-119">HTTP request</span></span>

<span data-ttu-id="4f7f5-120">[イベント](../resources/event.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-120">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="4f7f5-121">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-121">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="4f7f5-122">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-122">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="4f7f5-123">ユーザーのメールボックス内の[mailFolder](../resources/mailfolder.md)の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-123">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="4f7f5-124">次の例は、入れ子のレベルを 1 つを示していますが、メッセージというように子の子であることができます。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-124">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="4f7f5-125">[Outlook タスク](../resources/outlooktask.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-125">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="4f7f5-126">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-126">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f7f5-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4f7f5-127">Optional query parameters</span></span>

<span data-ttu-id="4f7f5-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f7f5-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f7f5-129">Request headers</span></span>

| <span data-ttu-id="4f7f5-130">名前</span><span class="sxs-lookup"><span data-stu-id="4f7f5-130">Name</span></span>       | <span data-ttu-id="4f7f5-131">型</span><span class="sxs-lookup"><span data-stu-id="4f7f5-131">Type</span></span> | <span data-ttu-id="4f7f5-132">説明</span><span class="sxs-lookup"><span data-stu-id="4f7f5-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f7f5-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f7f5-133">Authorization</span></span>  | <span data-ttu-id="4f7f5-134">string</span><span class="sxs-lookup"><span data-stu-id="4f7f5-134">string</span></span>  | <span data-ttu-id="4f7f5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f7f5-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f7f5-137">Request body</span></span>

<span data-ttu-id="4f7f5-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f7f5-139">応答</span><span class="sxs-lookup"><span data-stu-id="4f7f5-139">Response</span></span>

<span data-ttu-id="4f7f5-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-140">If successful, this method returns a `200 OK` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="4f7f5-141">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="4f7f5-141">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="4f7f5-142">要求</span><span class="sxs-lookup"><span data-stu-id="4f7f5-142">Request</span></span>

<span data-ttu-id="4f7f5-143">以下は、イベントの添付ファイルを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-143">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="4f7f5-144">応答</span><span class="sxs-lookup"><span data-stu-id="4f7f5-144">Response</span></span>

<span data-ttu-id="4f7f5-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "contentType": "contentType-value",
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="4f7f5-148">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="4f7f5-148">Example (item attachment)</span></span>

### <a name="request-1"></a><span data-ttu-id="4f7f5-149">要求 1</span><span class="sxs-lookup"><span data-stu-id="4f7f5-149">Request 1</span></span>

<span data-ttu-id="4f7f5-p106">最初の例は、メッセージの項目の添付ファイルを取得する方法を示しています。**itemAttachment** のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-p106">The first example shows how to get an item attachment on a message. The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_item_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```

### <a name="response-1"></a><span data-ttu-id="4f7f5-152">応答 1</span><span class="sxs-lookup"><span data-stu-id="4f7f5-152">Response 1</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="request-2"></a><span data-ttu-id="4f7f5-153">要求 2</span><span class="sxs-lookup"><span data-stu-id="4f7f5-153">Request 2</span></span>

<span data-ttu-id="4f7f5-p107">次の例は、`$expand` を使用してメッセージに添付されている項目のプロパティを取得する方法を示しています。この例では、項目はメッセージであり、添付メッセージのプロパティも返されます。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-p107">The next example shows how to use `$expand` to get the properties of the item that is attached to the message. In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```

### <a name="response-2"></a><span data-ttu-id="4f7f5-156">応答 2</span><span class="sxs-lookup"><span data-stu-id="4f7f5-156">Response 2</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="4f7f5-157">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="4f7f5-157">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="4f7f5-158">要求</span><span class="sxs-lookup"><span data-stu-id="4f7f5-158">Request</span></span>

<span data-ttu-id="4f7f5-159">以下は、イベントの添付ファイルの参照を取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4f7f5-159">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```

### <a name="response"></a><span data-ttu-id="4f7f5-160">応答</span><span class="sxs-lookup"><span data-stu-id="4f7f5-160">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/attachment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
