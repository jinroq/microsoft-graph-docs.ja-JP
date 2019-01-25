---
title: 添付ファイルを削除する
description: カレンダー イベント、メッセージ、Outlook のタスク、または投稿の添付ファイルを削除します。
localization_priority: Normal
ms.openlocfilehash: 5bb24fc97a2f99dbb0fbec77e2de941f770c27fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510898"
---
# <a name="delete-attachment"></a><span data-ttu-id="26fe0-103">添付ファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="26fe0-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26fe0-104">カレンダー[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[投稿](../resources/post.md)の添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="26fe0-104">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26fe0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26fe0-105">Permissions</span></span>

<span data-ttu-id="26fe0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26fe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="26fe0-108">メッセージの添付ファイルにアクセスする場合:Mail.ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="26fe0-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="26fe0-109">イベントの添付ファイルにアクセスする場合:Calendars.ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="26fe0-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="26fe0-110">Outlook からのタスクの添付ファイルにアクセスする場合: Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26fe0-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="26fe0-111">グループの投稿の添付ファイルにアクセスする場合: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26fe0-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="26fe0-112">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26fe0-112">HTTP request</span></span>

<span data-ttu-id="26fe0-113">[イベント](../resources/event.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="26fe0-113">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="26fe0-114">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="26fe0-114">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="26fe0-115">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="26fe0-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="26fe0-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="26fe0-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. <!-- { "blockType": "ignored" } --></span></span>

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="26fe0-118">[Outlook タスク](../resources/outlooktask.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="26fe0-118">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="26fe0-119">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="26fe0-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26fe0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26fe0-120">Request headers</span></span>

| <span data-ttu-id="26fe0-121">名前</span><span class="sxs-lookup"><span data-stu-id="26fe0-121">Name</span></span>       | <span data-ttu-id="26fe0-122">型</span><span class="sxs-lookup"><span data-stu-id="26fe0-122">Type</span></span> | <span data-ttu-id="26fe0-123">説明</span><span class="sxs-lookup"><span data-stu-id="26fe0-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26fe0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="26fe0-124">Authorization</span></span>  | <span data-ttu-id="26fe0-125">string</span><span class="sxs-lookup"><span data-stu-id="26fe0-125">string</span></span>  | <span data-ttu-id="26fe0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26fe0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26fe0-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="26fe0-128">Request body</span></span>

<span data-ttu-id="26fe0-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="26fe0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26fe0-130">応答</span><span class="sxs-lookup"><span data-stu-id="26fe0-130">Response</span></span>

<span data-ttu-id="26fe0-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="26fe0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26fe0-133">例</span><span class="sxs-lookup"><span data-stu-id="26fe0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="26fe0-134">要求</span><span class="sxs-lookup"><span data-stu-id="26fe0-134">Request</span></span>

<span data-ttu-id="26fe0-135">以下は、イベントの添付ファイルを削除する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26fe0-135">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="26fe0-136">応答</span><span class="sxs-lookup"><span data-stu-id="26fe0-136">Response</span></span>

<span data-ttu-id="26fe0-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="26fe0-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/attachment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
