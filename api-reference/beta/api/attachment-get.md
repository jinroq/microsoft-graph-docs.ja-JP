---
title: 添付ファイルを取得する
description: 'プロパティとイベントに関連付けられている添付ファイルの関係を読み取る '
ms.openlocfilehash: a432e4f3fb98062a701e4c6e7b177145faa65e1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068033"
---
# <a name="get-attachment"></a><span data-ttu-id="f0573-103">添付ファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="f0573-103">Get attachment</span></span>

> <span data-ttu-id="f0573-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0573-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0573-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0573-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0573-106">プロパティと[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付された添付ファイルの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0573-106">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="f0573-107">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="f0573-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="f0573-108">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="f0573-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="f0573-p102">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)。`$expand` を使用すると、その項目のプロパティをさらに取得できます。次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0573-p102">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource). You can use `$expand` to further get the properties of that item. See an [example](#request-2) below.</span></span>
* <span data-ttu-id="f0573-112">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="f0573-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="f0573-113">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="f0573-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f0573-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0573-114">Permissions</span></span>
<span data-ttu-id="f0573-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0573-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f0573-117">メッセージの添付ファイルにアクセスする場合: Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f0573-117">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="f0573-118">イベントで添付ファイルにアクセスする場合: Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f0573-118">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="f0573-119">Outlook からのタスクの添付ファイルにアクセスする場合: Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f0573-119">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="f0573-120">グループの投稿の添付ファイルにアクセスする場合: Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0573-120">If accessing attachments in group posts: Group.Read.All</span></span>
<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="f0573-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0573-121">HTTP request</span></span>
<span data-ttu-id="f0573-122">ユーザーの既定の[予定表](../resources/calendar.md)に[イベント](../resources/event.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="f0573-122">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}

GET /me/calendar/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="f0573-123">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f0573-123">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="f0573-124">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f0573-124">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="f0573-125">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f0573-125">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="f0573-126">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f0573-126">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="f0573-127">ユーザーのメールボックス内の[mailFolder](../resources/mailfolder.md)の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="f0573-127">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="f0573-128">次の例は、入れ子のレベルを 1 つを示していますが、メッセージというように子の子であることができます。</span><span class="sxs-lookup"><span data-stu-id="f0573-128">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="f0573-129">[Outlook タスク](../resources/outlooktask.md)またはフォルダーを指定したタスクまたはタスク グループで、ユーザーのメールボックス内の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="f0573-129">Attachments for an [Outlook task](../resources/outlooktask.md) in the user's mailbox, or in a specified task folder or task group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/tasks/<id>/attachments/{id}

GET /me/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}

GET /me/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
```

<span data-ttu-id="f0573-130">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f0573-130">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0573-131">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f0573-131">Optional query parameters</span></span>
<span data-ttu-id="f0573-132">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f0573-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0573-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0573-133">Request headers</span></span>
| <span data-ttu-id="f0573-134">名前</span><span class="sxs-lookup"><span data-stu-id="f0573-134">Name</span></span>       | <span data-ttu-id="f0573-135">型</span><span class="sxs-lookup"><span data-stu-id="f0573-135">Type</span></span> | <span data-ttu-id="f0573-136">説明</span><span class="sxs-lookup"><span data-stu-id="f0573-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f0573-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0573-137">Authorization</span></span>  | <span data-ttu-id="f0573-138">string</span><span class="sxs-lookup"><span data-stu-id="f0573-138">string</span></span>  | <span data-ttu-id="f0573-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0573-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0573-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0573-141">Request body</span></span>
<span data-ttu-id="f0573-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f0573-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0573-143">応答</span><span class="sxs-lookup"><span data-stu-id="f0573-143">Response</span></span>

<span data-ttu-id="f0573-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0573-144">If successful, this method returns a `200 OK` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f0573-145">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="f0573-145">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f0573-146">要求</span><span class="sxs-lookup"><span data-stu-id="f0573-146">Request</span></span>
<span data-ttu-id="f0573-147">以下は、イベントの添付ファイルを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0573-147">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

##### <a name="response"></a><span data-ttu-id="f0573-148">応答</span><span class="sxs-lookup"><span data-stu-id="f0573-148">Response</span></span>
<span data-ttu-id="f0573-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0573-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
## <a name="example-item-attachment"></a><span data-ttu-id="f0573-152">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="f0573-152">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="f0573-153">要求 1</span><span class="sxs-lookup"><span data-stu-id="f0573-153">Request 1</span></span>
<span data-ttu-id="f0573-p107">最初の例は、メッセージの項目の添付ファイルを取得する方法を示しています。**itemAttachment** のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f0573-p107">The first example shows how to get an item attachment on a message. The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```

##### <a name="response-1"></a><span data-ttu-id="f0573-156">応答 1</span><span class="sxs-lookup"><span data-stu-id="f0573-156">Response 1</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="f0573-157">要求 2</span><span class="sxs-lookup"><span data-stu-id="f0573-157">Request 2</span></span>
<span data-ttu-id="f0573-p108">次の例は、`$expand` を使用してメッセージに添付されている項目のプロパティを取得する方法を示しています。この例では、項目はメッセージであり、添付メッセージのプロパティも返されます。</span><span class="sxs-lookup"><span data-stu-id="f0573-p108">The next example shows how to use `$expand` to get the properties of the item that is attached to the message. In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item 
```

##### <a name="response-2"></a><span data-ttu-id="f0573-160">応答 2</span><span class="sxs-lookup"><span data-stu-id="f0573-160">Response 2</span></span>
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


## <a name="example-reference-attachment"></a><span data-ttu-id="f0573-161">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="f0573-161">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f0573-162">要求</span><span class="sxs-lookup"><span data-stu-id="f0573-162">Request</span></span>
<span data-ttu-id="f0573-163">以下は、イベントの添付ファイルの参照を取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0573-163">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```

##### <a name="response"></a><span data-ttu-id="f0573-164">応答</span><span class="sxs-lookup"><span data-stu-id="f0573-164">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
