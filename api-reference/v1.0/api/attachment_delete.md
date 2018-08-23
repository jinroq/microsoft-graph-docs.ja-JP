# <a name="delete-attachment"></a><span data-ttu-id="97468-101">添付ファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="97468-101">Delete attachment</span></span>

<span data-ttu-id="97468-102">予定表イベント、メール メッセージ、またはグループ投稿から添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="97468-102">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="97468-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="97468-103">Permissions</span></span>
<span data-ttu-id="97468-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、[アクセス許可](../../../concepts/permissions_reference.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97468-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="97468-106">メッセージの添付ファイルにアクセスする場合: Mail.ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="97468-106">If accessing attachments in Messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="97468-107">イベントの添付ファイルにアクセスする場合: Calendars.ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="97468-107">If accessing attachments in Events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="97468-108">グループの投稿の添付ファイルにアクセスする場合: Group.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="97468-108">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="97468-109">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97468-109">HTTP request</span></span>
<span data-ttu-id="97468-110">ユーザーまたはグループの既定の[カレンダー](../resources/calendar.md)内の[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="97468-110">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
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

<span data-ttu-id="97468-111">ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="97468-111">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="97468-112">ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="97468-112">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="97468-113">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="97468-113">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="97468-114">ユーザーのメールボックスの最上位レベルの[mailFolder](../resources/mailfolder.md)に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="97468-114">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="97468-115">ユーザーのメールボックス内の[mailFolder](../resources/mailfolder.md)の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="97468-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="97468-116">次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="97468-116">A contact contained in a child folder of a contactFolder. The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="97468-117">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="97468-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="97468-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97468-118">Request headers</span></span>
| <span data-ttu-id="97468-119">名前</span><span class="sxs-lookup"><span data-stu-id="97468-119">Name</span></span>       | <span data-ttu-id="97468-120">型</span><span class="sxs-lookup"><span data-stu-id="97468-120">Type</span></span> | <span data-ttu-id="97468-121">説明</span><span class="sxs-lookup"><span data-stu-id="97468-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97468-122">承認</span><span class="sxs-lookup"><span data-stu-id="97468-122">Authorization</span></span>  | <span data-ttu-id="97468-123">文字列</span><span class="sxs-lookup"><span data-stu-id="97468-123">string</span></span>  | <span data-ttu-id="97468-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="97468-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97468-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="97468-126">Request body</span></span>
<span data-ttu-id="97468-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="97468-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97468-128">応答</span><span class="sxs-lookup"><span data-stu-id="97468-128">Response</span></span>

<span data-ttu-id="97468-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="97468-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97468-131">例</span><span class="sxs-lookup"><span data-stu-id="97468-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97468-132">要求</span><span class="sxs-lookup"><span data-stu-id="97468-132">Request</span></span>
<span data-ttu-id="97468-133">以下は、イベントの添付ファイルを削除する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="97468-133">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="97468-134">応答</span><span class="sxs-lookup"><span data-stu-id="97468-134">Response</span></span>
<span data-ttu-id="97468-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="97468-135">Here is an example of the response.</span></span>
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
