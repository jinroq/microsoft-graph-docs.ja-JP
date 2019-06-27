---
title: 添付ファイルを削除する
description: 予定表イベント、メール メッセージ、またはグループ投稿から添付ファイルを削除します。
localization_priority: Normal
ms.openlocfilehash: aa1a031826c4e0875007ba63ea8cf21695d8e49b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272668"
---
# <a name="delete-attachment"></a><span data-ttu-id="b66cd-103">添付ファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="b66cd-103">Delete attachment</span></span>

<span data-ttu-id="b66cd-104">予定表イベント、メール メッセージ、またはグループ投稿から添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="b66cd-104">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="b66cd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b66cd-105">Permissions</span></span>
<span data-ttu-id="b66cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b66cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="b66cd-108">メッセージ内の添付ファイルにアクセスする場合: 「メールの書き込み」。</span><span class="sxs-lookup"><span data-stu-id="b66cd-108">If accessing attachments in messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="b66cd-109">イベントの添付ファイルにアクセスする場合: 「カレンダー」。</span><span class="sxs-lookup"><span data-stu-id="b66cd-109">If accessing attachments in events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="b66cd-110">グループの投稿で添付ファイルにアクセスする場合: グループの場合。</span><span class="sxs-lookup"><span data-stu-id="b66cd-110">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="b66cd-111">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b66cd-111">HTTP request</span></span>
<span data-ttu-id="b66cd-112">ユーザーまたはグループの既定の[カレンダー](../resources/calendar.md)内の[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="b66cd-112">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
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

<span data-ttu-id="b66cd-113">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="b66cd-113">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="b66cd-114">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="b66cd-114">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="b66cd-115">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="b66cd-115">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b66cd-116">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="b66cd-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b66cd-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="b66cd-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b66cd-119">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="b66cd-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b66cd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b66cd-120">Request headers</span></span>
| <span data-ttu-id="b66cd-121">名前</span><span class="sxs-lookup"><span data-stu-id="b66cd-121">Name</span></span>       | <span data-ttu-id="b66cd-122">型</span><span class="sxs-lookup"><span data-stu-id="b66cd-122">Type</span></span> | <span data-ttu-id="b66cd-123">説明</span><span class="sxs-lookup"><span data-stu-id="b66cd-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b66cd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b66cd-124">Authorization</span></span>  | <span data-ttu-id="b66cd-125">string</span><span class="sxs-lookup"><span data-stu-id="b66cd-125">string</span></span>  | <span data-ttu-id="b66cd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b66cd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b66cd-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b66cd-128">Request body</span></span>
<span data-ttu-id="b66cd-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b66cd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b66cd-130">応答</span><span class="sxs-lookup"><span data-stu-id="b66cd-130">Response</span></span>

<span data-ttu-id="b66cd-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b66cd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b66cd-133">例</span><span class="sxs-lookup"><span data-stu-id="b66cd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b66cd-134">要求</span><span class="sxs-lookup"><span data-stu-id="b66cd-134">Request</span></span>
<span data-ttu-id="b66cd-135">以下は、イベントの添付ファイルを削除する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b66cd-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="b66cd-136">応答</span><span class="sxs-lookup"><span data-stu-id="b66cd-136">Response</span></span>
<span data-ttu-id="b66cd-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b66cd-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b66cd-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="b66cd-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b66cd-139">C#</span><span class="sxs-lookup"><span data-stu-id="b66cd-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b66cd-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="b66cd-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b66cd-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="b66cd-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
