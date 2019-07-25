---
title: 添付ファイルを取得する
description: 'イベントに添付されている添付ファイルのプロパティとリレーションシップを読み取ります。 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8e61b57bd619bbd9cb9a213db2d89d1557b201f3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882622"
---
# <a name="get-attachment"></a><span data-ttu-id="f536a-103">添付ファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="f536a-103">Get attachment</span></span>

<span data-ttu-id="f536a-104">[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、または[投稿](../resources/post.md)に添付されている添付ファイルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f536a-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="f536a-105">添付ファイルには、次の種類のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="f536a-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="f536a-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="f536a-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="f536a-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="f536a-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="f536a-108">`$expand` を使用すると、その項目のプロパティをさらに取得できます。</span><span class="sxs-lookup"><span data-stu-id="f536a-108">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="f536a-109">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f536a-109">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="f536a-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="f536a-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="f536a-111">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="f536a-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 


## <a name="permissions"></a><span data-ttu-id="f536a-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f536a-112">Permissions</span></span>
<span data-ttu-id="f536a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f536a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f536a-115">メッセージの添付ファイルにアクセスする場合: Mail.Read。</span><span class="sxs-lookup"><span data-stu-id="f536a-115">If accessing attachments in Messages: Mail.Read</span></span>
* <span data-ttu-id="f536a-116">イベントの添付ファイルにアクセスする場合: Calendars.Read。</span><span class="sxs-lookup"><span data-stu-id="f536a-116">If accessing attachments in Events: Calendars.Read</span></span>
* <span data-ttu-id="f536a-117">グループ投稿の添付ファイルにアクセスする場合: Group.Read.All。</span><span class="sxs-lookup"><span data-stu-id="f536a-117">If accessing attachments in group events or posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="f536a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f536a-118">HTTP request</span></span>
<span data-ttu-id="f536a-119">ユーザーの既定の[カレンダー](../resources/calendar.md)内の[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f536a-119">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="f536a-120">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f536a-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="f536a-121">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f536a-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="f536a-122">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f536a-122">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="f536a-123">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f536a-123">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="f536a-p103">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。 </span><span class="sxs-lookup"><span data-stu-id="f536a-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="f536a-126">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="f536a-126">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f536a-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f536a-127">Optional query parameters</span></span>
<span data-ttu-id="f536a-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f536a-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f536a-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f536a-129">Request headers</span></span>
| <span data-ttu-id="f536a-130">名前</span><span class="sxs-lookup"><span data-stu-id="f536a-130">Name</span></span>       | <span data-ttu-id="f536a-131">型</span><span class="sxs-lookup"><span data-stu-id="f536a-131">Type</span></span> | <span data-ttu-id="f536a-132">説明</span><span class="sxs-lookup"><span data-stu-id="f536a-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f536a-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="f536a-133">Authorization</span></span>  | <span data-ttu-id="f536a-134">string</span><span class="sxs-lookup"><span data-stu-id="f536a-134">string</span></span>  | <span data-ttu-id="f536a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f536a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f536a-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="f536a-137">Request body</span></span>
<span data-ttu-id="f536a-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f536a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f536a-139">応答</span><span class="sxs-lookup"><span data-stu-id="f536a-139">Response</span></span>

<span data-ttu-id="f536a-140">成功した場合、このメソッドは `200 OK` 応答コードと応答本文で **Attachment** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f536a-140">If successful, this method returns a `200 OK` response code and **attachment** object in the response body.</span></span> <span data-ttu-id="f536a-141">その種類の添付ファイル ([fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md)、または [referenceAttachment](../resources/referenceattachment.md)) のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f536a-141">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f536a-142">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="f536a-142">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f536a-143">要求</span><span class="sxs-lookup"><span data-stu-id="f536a-143">Request</span></span>
<span data-ttu-id="f536a-144">以下は、イベントの添付ファイルを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f536a-144">Here is an example of the request to get a file attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f536a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f536a-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f536a-146">C#</span><span class="sxs-lookup"><span data-stu-id="f536a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f536a-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="f536a-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f536a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f536a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f536a-149">Java</span><span class="sxs-lookup"><span data-stu-id="f536a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f536a-150">応答</span><span class="sxs-lookup"><span data-stu-id="f536a-150">Response</span></span>
<span data-ttu-id="f536a-p106">以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f536a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "contentBytes": "binary",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```
## <a name="example-item-attachment"></a><span data-ttu-id="f536a-154">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="f536a-154">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="f536a-155">要求 1</span><span class="sxs-lookup"><span data-stu-id="f536a-155">Request 1</span></span>
<span data-ttu-id="f536a-156">最初の例は、メッセージの項目の添付ファイルを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f536a-156">The first example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="f536a-157">**itemAttachment** のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f536a-157">The properties of the **itemAttachment** are returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f536a-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="f536a-158">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f536a-159">C#</span><span class="sxs-lookup"><span data-stu-id="f536a-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f536a-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="f536a-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f536a-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f536a-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f536a-162">Java</span><span class="sxs-lookup"><span data-stu-id="f536a-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="f536a-163">応答 1</span><span class="sxs-lookup"><span data-stu-id="f536a-163">Response 1</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

##### <a name="request-2"></a><span data-ttu-id="f536a-164">要求 2</span><span class="sxs-lookup"><span data-stu-id="f536a-164">Request 2</span></span>
<span data-ttu-id="f536a-165">次の例は、`$expand` を使用してメッセージに添付されている項目のプロパティを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f536a-165">The next example shows how to use `$expand` to get the properties of the item that is attached to the message.</span></span> <span data-ttu-id="f536a-166">この例では、項目はメッセージであり、添付メッセージのプロパティも返されます。</span><span class="sxs-lookup"><span data-stu-id="f536a-166">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f536a-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="f536a-167">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f536a-168">C#</span><span class="sxs-lookup"><span data-stu-id="f536a-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f536a-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="f536a-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f536a-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f536a-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f536a-171">Java</span><span class="sxs-lookup"><span data-stu-id="f536a-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="f536a-172">応答 2</span><span class="sxs-lookup"><span data-stu-id="f536a-172">Response 2</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
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
    ]
  }
}
```



## <a name="example-reference-attachment"></a><span data-ttu-id="f536a-173">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="f536a-173">Example (reference attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="f536a-174">要求</span><span class="sxs-lookup"><span data-stu-id="f536a-174">Request</span></span>
<span data-ttu-id="f536a-175">以下は、メッセージの参照添付ファイルを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f536a-175">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f536a-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="f536a-176">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f536a-177">C#</span><span class="sxs-lookup"><span data-stu-id="f536a-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f536a-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="f536a-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f536a-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f536a-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f536a-180">Java</span><span class="sxs-lookup"><span data-stu-id="f536a-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f536a-181">応答</span><span class="sxs-lookup"><span data-stu-id="f536a-181">Response</span></span>
<span data-ttu-id="f536a-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f536a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_reference_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKgAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=",
    "lastModifiedDateTime": "2019-04-02T02:58:11Z",
    "name": "Sales Invoice Template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 1060,
    "isInline": true
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_and_expand_item_attachment/item:
      Property 'item' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
