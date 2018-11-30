---
title: 添付ファイルを削除する
description: 予定表のイベントでは、添付ファイルを削除します。
ms.openlocfilehash: 5e5fe0205e667908947993b01388f90c1688c95e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067053"
---
# <a name="delete-attachment"></a><span data-ttu-id="ce62a-103">添付ファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="ce62a-103">Delete attachment</span></span>

> <span data-ttu-id="ce62a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce62a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce62a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce62a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce62a-106">カレンダー[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[投稿](../resources/post.md)の添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="ce62a-106">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ce62a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce62a-107">Permissions</span></span>
<span data-ttu-id="ce62a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce62a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="ce62a-110">メッセージの添付ファイルにアクセスする場合: Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce62a-110">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="ce62a-111">イベントで添付ファイルにアクセスする場合: Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce62a-111">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="ce62a-112">Outlook からのタスクの添付ファイルにアクセスする場合: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce62a-112">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="ce62a-113">グループの投稿の添付ファイルにアクセスする場合: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce62a-113">If accessing attachments in group posts: Group.ReadWrite.All</span></span>
<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="ce62a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce62a-114">HTTP request</span></span>
<span data-ttu-id="ce62a-115">ユーザーの既定の[予定表](../resources/calendar.md)に[イベント](../resources/event.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="ce62a-115">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
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

<span data-ttu-id="ce62a-116">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="ce62a-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="ce62a-117">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="ce62a-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="ce62a-118">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="ce62a-118">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="ce62a-119">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="ce62a-119">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="ce62a-120">ユーザーのメールボックス内の[mailFolder](../resources/mailfolder.md)の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="ce62a-120">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="ce62a-121">次の例は、入れ子のレベルを 1 つを示していますが、メッセージというように子の子であることができます。</span><span class="sxs-lookup"><span data-stu-id="ce62a-121">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="ce62a-122">[Outlook タスク](../resources/outlooktask.md)またはフォルダーを指定したタスクまたはタスク グループで、ユーザーのメールボックス内の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="ce62a-122">Attachments for an [Outlook task](../resources/outlooktask.md) in the user's mailbox, or in a specified task folder or task group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}

DELETE /me/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}

DELETE /me/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
```

<span data-ttu-id="ce62a-123">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="ce62a-123">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ce62a-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce62a-124">Request headers</span></span>
| <span data-ttu-id="ce62a-125">名前</span><span class="sxs-lookup"><span data-stu-id="ce62a-125">Name</span></span>       | <span data-ttu-id="ce62a-126">型</span><span class="sxs-lookup"><span data-stu-id="ce62a-126">Type</span></span> | <span data-ttu-id="ce62a-127">説明</span><span class="sxs-lookup"><span data-stu-id="ce62a-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ce62a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce62a-128">Authorization</span></span>  | <span data-ttu-id="ce62a-129">string</span><span class="sxs-lookup"><span data-stu-id="ce62a-129">string</span></span>  | <span data-ttu-id="ce62a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce62a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce62a-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce62a-132">Request body</span></span>
<span data-ttu-id="ce62a-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce62a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce62a-134">応答</span><span class="sxs-lookup"><span data-stu-id="ce62a-134">Response</span></span>

<span data-ttu-id="ce62a-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ce62a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce62a-137">例</span><span class="sxs-lookup"><span data-stu-id="ce62a-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce62a-138">要求</span><span class="sxs-lookup"><span data-stu-id="ce62a-138">Request</span></span>
<span data-ttu-id="ce62a-139">以下は、イベントの添付ファイルを削除する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce62a-139">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="ce62a-140">応答</span><span class="sxs-lookup"><span data-stu-id="ce62a-140">Response</span></span>
<span data-ttu-id="ce62a-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ce62a-141">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
