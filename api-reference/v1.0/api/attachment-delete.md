---
title: 添付ファイルを削除する
description: 予定表イベント、メール メッセージ、またはグループ投稿から添付ファイルを削除します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 78b8fd39741fb58b4386a70bc463de2cf4a4d546
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347718"
---
# <a name="delete-attachment"></a><span data-ttu-id="5bbe6-103">添付ファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="5bbe6-103">Delete attachment</span></span>

<span data-ttu-id="5bbe6-104">予定表イベント、メール メッセージ、またはグループ投稿から添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-104">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="5bbe6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5bbe6-105">Permissions</span></span>
<span data-ttu-id="5bbe6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="5bbe6-108">メッセージ内の添付ファイルにアクセスする場合: 「メールの書き込み」。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-108">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="5bbe6-109">イベントの添付ファイルにアクセスする場合: 「カレンダー」。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-109">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="5bbe6-110">グループの投稿で添付ファイルにアクセスする場合: グループの場合。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-110">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="5bbe6-111">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bbe6-111">HTTP request</span></span>
<span data-ttu-id="5bbe6-112">ユーザーまたはグループの既定の[カレンダー](../resources/calendar.md)内の[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-112">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="5bbe6-113">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-113">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="5bbe6-114">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-114">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="5bbe6-115">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="5bbe6-116">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="5bbe6-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="5bbe6-119">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5bbe6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bbe6-120">Request headers</span></span>
| <span data-ttu-id="5bbe6-121">名前</span><span class="sxs-lookup"><span data-stu-id="5bbe6-121">Name</span></span>       | <span data-ttu-id="5bbe6-122">型</span><span class="sxs-lookup"><span data-stu-id="5bbe6-122">Type</span></span> | <span data-ttu-id="5bbe6-123">説明</span><span class="sxs-lookup"><span data-stu-id="5bbe6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5bbe6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bbe6-124">Authorization</span></span>  | <span data-ttu-id="5bbe6-125">string</span><span class="sxs-lookup"><span data-stu-id="5bbe6-125">string</span></span>  | <span data-ttu-id="5bbe6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bbe6-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bbe6-128">Request body</span></span>
<span data-ttu-id="5bbe6-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bbe6-130">応答</span><span class="sxs-lookup"><span data-stu-id="5bbe6-130">Response</span></span>

<span data-ttu-id="5bbe6-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bbe6-133">例</span><span class="sxs-lookup"><span data-stu-id="5bbe6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bbe6-134">要求</span><span class="sxs-lookup"><span data-stu-id="5bbe6-134">Request</span></span>
<span data-ttu-id="5bbe6-135">以下は、イベントの添付ファイルを削除する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-135">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5bbe6-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5bbe6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5bbe6-137">C#</span><span class="sxs-lookup"><span data-stu-id="5bbe6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bbe6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bbe6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5bbe6-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="5bbe6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5bbe6-140">Java</span><span class="sxs-lookup"><span data-stu-id="5bbe6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5bbe6-141">応答</span><span class="sxs-lookup"><span data-stu-id="5bbe6-141">Response</span></span>
<span data-ttu-id="5bbe6-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5bbe6-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
