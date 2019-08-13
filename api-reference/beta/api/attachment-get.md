---
title: 添付ファイルを取得する
description: イベント、メッセージ、Outlook タスク、または投稿に添付されている添付ファイルのプロパティとリレーションシップを読み取ります。
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f394c3a80a6d0dad328403ea96732a5afd146130
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318545"
---
# <a name="get-attachment"></a><span data-ttu-id="c0bdd-103">添付ファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-103">Get attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0bdd-104">[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook タスク](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付されている添付ファイルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

<span data-ttu-id="c0bdd-105">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="c0bdd-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="c0bdd-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="c0bdd-108">を使用`$expand`して、そのアイテムのプロパティをさらに取得することができます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-108">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="c0bdd-109">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-109">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="c0bdd-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="c0bdd-111">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span>

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="c0bdd-112">ファイルまたはアイテムの添付ファイルの生のコンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-112">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="c0bdd-113">パスセグメント`/$value`を追加して、ファイルまたはアイテムの添付ファイルの生のコンテンツを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-113">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="c0bdd-114">添付ファイルの場合、コンテンツタイプは、元のコンテンツタイプに基づいています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-114">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="c0bdd-115">次の[例](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-115">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="c0bdd-116">[連絡先](../resources/contact.md)、[イベント](../resources/event.md)、または[メッセージ](../resources/message.md)であるアイテムの添付ファイルの場合、返される生のコンテンツは MIME 形式です。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-116">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="c0bdd-117">アイテムの添付ファイルの種類</span><span class="sxs-lookup"><span data-stu-id="c0bdd-117">Item attachment type</span></span>  | <span data-ttu-id="c0bdd-118">返された生のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="c0bdd-118">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c0bdd-119">**contact**</span><span class="sxs-lookup"><span data-stu-id="c0bdd-119">**contact**</span></span> | <span data-ttu-id="c0bdd-120">[vCard](http://www.faqs.org/rfcs/rfc2426.html)MIME 形式。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-120">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="c0bdd-121">[例](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-121">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="c0bdd-122">**event**</span><span class="sxs-lookup"><span data-stu-id="c0bdd-122">**event**</span></span> | <span data-ttu-id="c0bdd-123">iCal MIME 形式。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-123">iCal MIME format.</span></span> <span data-ttu-id="c0bdd-124">[例](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-124">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="c0bdd-125">**message**</span><span class="sxs-lookup"><span data-stu-id="c0bdd-125">**message**</span></span> | <span data-ttu-id="c0bdd-126">MIME 形式。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-126">MIME format.</span></span> <span data-ttu-id="c0bdd-127">[例](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-127">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="c0bdd-128">参照添付ファイルの`$value`を取得しようとすると、HTTP 405 が返されます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-128">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0bdd-129">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0bdd-129">Permissions</span></span>

<span data-ttu-id="c0bdd-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="c0bdd-132">メッセージの添付ファイルにアクセスする場合: Mail. 読み取り</span><span class="sxs-lookup"><span data-stu-id="c0bdd-132">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="c0bdd-133">イベントの添付ファイルにアクセスする場合: 予定表. 読み取り</span><span class="sxs-lookup"><span data-stu-id="c0bdd-133">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="c0bdd-134">Outlook のタスクで添付ファイルにアクセスする場合: Tasks. 読み取り</span><span class="sxs-lookup"><span data-stu-id="c0bdd-134">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="c0bdd-135">グループの投稿で添付ファイルにアクセスする場合: グループの全員</span><span class="sxs-lookup"><span data-stu-id="c0bdd-135">If accessing attachments in group posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="c0bdd-136">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-136">HTTP request</span></span>

<span data-ttu-id="c0bdd-137">このセクションでは、添付ファイルをサポートする各エンティティ ([イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook タスク](../resources/outlooktask.md)、または[post](../resources/post.md)) の HTTP GET 要求構文を示します。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-137">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="c0bdd-138">添付ファイルのプロパティとリレーションシップを取得するには、指定された[イベント](../resources/event.md)、 \*\*\*\* [メッセージ](../resources/message.md)、 [Outlook タスク](../resources/outlooktask.md)、または[post](../resources/post.md)インスタンスに添付された添付ファイルコレクションにインデックスを付ける添付ファイル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-138">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="c0bdd-139">添付ファイルがファイルまたは Outlook アイテム (連絡先、イベント、またはメッセージ) の場合は、パスセグメント`/$value`を要求 URL に追加することによって、添付ファイルの生のコンテンツをさらに取得できます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-139">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="c0bdd-140">[イベント](../resources/event.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-140">An attachment of an [event](../resources/event.md):</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="c0bdd-141">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル:</span><span class="sxs-lookup"><span data-stu-id="c0bdd-141">An attachment of a [message](../resources/message.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="c0bdd-142">ユーザーのメールボックス内のトップレベルの[Mailfolder](../resources/mailfolder.md)に含まれる[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-142">An attachment of a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="c0bdd-143">ユーザーのメールボックス内の[Mailfolder](../resources/mailfolder.md)の子フォルダーに含まれる[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-143">An attachment of a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="c0bdd-144">前の例では、入れ子の1つのレベルを示していますが、メッセージは子の子に配置することもできます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-144">The preceding example shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>

<span data-ttu-id="c0bdd-145">[Outlook タスク](../resources/outlooktask.md)の添付ファイル:</span><span class="sxs-lookup"><span data-stu-id="c0bdd-145">An attachment of an [Outlook task](../resources/outlooktask.md):</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="c0bdd-146">グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-146">An attachment of a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0bdd-147">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c0bdd-147">Optional query parameters</span></span>

<span data-ttu-id="c0bdd-148">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-148">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0bdd-149">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0bdd-149">Request headers</span></span>

| <span data-ttu-id="c0bdd-150">名前</span><span class="sxs-lookup"><span data-stu-id="c0bdd-150">Name</span></span>       | <span data-ttu-id="c0bdd-151">型</span><span class="sxs-lookup"><span data-stu-id="c0bdd-151">Type</span></span> | <span data-ttu-id="c0bdd-152">説明</span><span class="sxs-lookup"><span data-stu-id="c0bdd-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0bdd-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0bdd-153">Authorization</span></span>  | <span data-ttu-id="c0bdd-154">string</span><span class="sxs-lookup"><span data-stu-id="c0bdd-154">string</span></span>  | <span data-ttu-id="c0bdd-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0bdd-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0bdd-157">Request body</span></span>

<span data-ttu-id="c0bdd-158">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0bdd-159">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-159">Response</span></span>

<span data-ttu-id="c0bdd-160">成功した場合、GET メソッドは`200 OK`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-160">If successful, the GET method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="c0bdd-161">添付ファイルのプロパティとリレーションシップを取得している場合は、応答本文に[attachment](../resources/attachment.md)オブジェクトが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-161">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span>

<span data-ttu-id="c0bdd-162">ファイルまたはアイテムの添付ファイルの生のコンテンツを取得する場合、応答本文には添付ファイルの生の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-162">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="c0bdd-163">例</span><span class="sxs-lookup"><span data-stu-id="c0bdd-163">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="c0bdd-164">例 1: 添付ファイルのプロパティを取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-164">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="c0bdd-165">要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-165">Request</span></span>

<span data-ttu-id="c0bdd-166">以下は、メッセージの添付ファイルのプロパティを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-166">Here is an example of the request to get the properties of a file attachment on a message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0bdd-167">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c0bdd-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0bdd-168">C#</span><span class="sxs-lookup"><span data-stu-id="c0bdd-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0bdd-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0bdd-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0bdd-170">目的-C</span><span class="sxs-lookup"><span data-stu-id="c0bdd-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0bdd-171">Java</span><span class="sxs-lookup"><span data-stu-id="c0bdd-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c0bdd-172">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-172">Response</span></span>

<span data-ttu-id="c0bdd-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "id": "AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=",
    "lastModifiedDateTime": "2019-04-02T03:41:29Z",
    "name": "Draft sales invoice template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 13068,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "base64,UEsDBBQABgAIAAAAIQ4AAAAA"
}
```

### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="c0bdd-176">例 2: アイテムの添付ファイルのプロパティを取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-176">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="c0bdd-177">要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-177">Request</span></span>

<span data-ttu-id="c0bdd-178">最初の例は、メッセージのアイテムの添付ファイルを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-178">The first example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="c0bdd-179">**Itemattachment**のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-179">The properties of the **itemAttachment** are returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0bdd-180">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c0bdd-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0bdd-181">C#</span><span class="sxs-lookup"><span data-stu-id="c0bdd-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0bdd-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0bdd-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0bdd-183">目的-C</span><span class="sxs-lookup"><span data-stu-id="c0bdd-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0bdd-184">Java</span><span class="sxs-lookup"><span data-stu-id="c0bdd-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c0bdd-185">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-185">Response</span></span>
<span data-ttu-id="c0bdd-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1M-CJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="c0bdd-189">例 3: メッセージに添付されたアイテムのプロパティを展開して取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-189">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="c0bdd-190">要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-190">Request</span></span>

<span data-ttu-id="c0bdd-191">次の例は、を使用`$expand`して、メッセージに添付されているアイテム (イベント、メッセージ、Outlook タスク、または投稿) のプロパティを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-191">The next example shows how to use `$expand` to get the properties of the item (event, message, Outlook task, or post) that is attached to the message.</span></span> <span data-ttu-id="c0bdd-192">この例では、アイテムがメッセージであることを示します。添付されたメッセージのプロパティも返されます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-192">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0bdd-193">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c0bdd-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0bdd-194">C#</span><span class="sxs-lookup"><span data-stu-id="c0bdd-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0bdd-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0bdd-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0bdd-196">目的-C</span><span class="sxs-lookup"><span data-stu-id="c0bdd-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0bdd-197">Java</span><span class="sxs-lookup"><span data-stu-id="c0bdd-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c0bdd-198">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-198">Response</span></span>
<span data-ttu-id="c0bdd-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_and_expand_item_attachment",
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

### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="c0bdd-202">例 4: 参照添付ファイルのプロパティを取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-202">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="c0bdd-203">要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-203">Request</span></span>

<span data-ttu-id="c0bdd-204">以下は、イベントの添付ファイルの参照を取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-204">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0bdd-205">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c0bdd-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0bdd-206">C#</span><span class="sxs-lookup"><span data-stu-id="c0bdd-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0bdd-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0bdd-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0bdd-208">目的-C</span><span class="sxs-lookup"><span data-stu-id="c0bdd-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0bdd-209">Java</span><span class="sxs-lookup"><span data-stu-id="c0bdd-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c0bdd-210">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-210">Response</span></span>
<span data-ttu-id="c0bdd-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="c0bdd-214">例 5: メッセージの添付ファイルの生の内容を取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-214">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="c0bdd-215">要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-215">Request</span></span>

<span data-ttu-id="c0bdd-216">メッセージに添付されている Word ファイルの生の内容を取得する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-216">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="c0bdd-217">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-217">Response</span></span>
<span data-ttu-id="c0bdd-218">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-218">Here is an example of the response.</span></span> <span data-ttu-id="c0bdd-219">実際の応答本文には、ファイル添付の生バイトが含まれており、簡潔にするためにここで短縮されています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-219">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="c0bdd-220">例 6: メッセージの連絡先添付ファイルの MIME 生の内容を取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-220">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="c0bdd-221">要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-221">Request</span></span>

<span data-ttu-id="c0bdd-222">メッセージに添付されている連絡先アイテムの生のコンテンツを取得する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-222">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="c0bdd-223">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-223">Response</span></span>
<span data-ttu-id="c0bdd-224">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-224">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCARD
PROFILE:VCARD
VERSION:3.0
MAILER:Microsoft Exchange
PRODID:Microsoft Exchange
FN:Alex Wilbur
N:Wilbur;Alex;;;
NOTE:Sunday\, June 10\, 2012 5:44 PM:\nGutter\, window cleaning\, pressure 
 washing\, roof debris blowing\n
ORG:Contoso;
CLASS:PUBLIC
ADR;TYPE=WORK,PREF:;;4567 Main St;Buffalo;NY;98052;United States of America
LABEL;TYPE=WORK,PREF:4567 Main St\nBuffalo\, NY 98052
ADR;TYPE=HOME:;;;;;;
ADR;TYPE=POSTAL:;;;;;;
TEL;TYPE=WORK:(425) 555-0100
TITLE:
X-MS-IMADDRESS:
REV;VALUE=DATE-TIME:2019-04-09T02:13:31,161Z
END:VCARD
```


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="c0bdd-225">例 7: メッセージのイベント添付ファイルの MIME 生の内容を取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-225">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="c0bdd-226">要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-226">Request</span></span>

<span data-ttu-id="c0bdd-227">メッセージに添付されているイベントの生の内容を取得する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-227">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="c0bdd-228">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-228">Response</span></span>
<span data-ttu-id="c0bdd-229">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-229">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCALENDAR
METHOD:PUBLISH
PRODID:Microsoft Exchange Server 2010
VERSION:2.0
BEGIN:VTIMEZONE
TZID:Pacific Standard Time
BEGIN:STANDARD
DTSTART:16010101T020000
TZOFFSETFROM:-0700
TZOFFSETTO:-0800
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=1SU;BYMONTH=11
END:STANDARD
BEGIN:DAYLIGHT
DTSTART:16010101T020000
TZOFFSETFROM:-0800
TZOFFSETTO:-0700
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=2SU;BYMONTH=3
END:DAYLIGHT
END:VTIMEZONE
BEGIN:VEVENT
ORGANIZER;CN=Adele Vance:MAILTO:adelev@contoso.com
ATTENDEE;ROLE=REQ-PARTICIPANT;PARTSTAT=NEEDS-ACTION;RSVP=TRUE;CN=Adele Vance:MAILTO:adelev@contoso.com
DESCRIPTION;LANGUAGE=en-US:\n
UID:040000008200
SUMMARY;LANGUAGE=en-US:Review Megan's docs
DTSTART;TZID=Pacific Standard Time:20190409T140000
DTEND;TZID=Pacific Standard Time:20190409T160000
CLASS:PUBLIC
PRIORITY:5
DTSTAMP:20190409T211833Z
TRANSP:OPAQUE
STATUS:CONFIRMED
SEQUENCE:0
LOCATION;LANGUAGE=en-US:
X-MICROSOFT-CDO-APPT-SEQUENCE:0
X-MICROSOFT-CDO-OWNERAPPTID:0
X-MICROSOFT-CDO-BUSYSTATUS:BUSY
X-MICROSOFT-CDO-INTENDEDSTATUS:BUSY
X-MICROSOFT-CDO-ALLDAYEVENT:FALSE
X-MICROSOFT-CDO-IMPORTANCE:1
X-MICROSOFT-CDO-INSTTYPE:0
X-MICROSOFT-DONOTFORWARDMEETING:FALSE
X-MICROSOFT-DISALLOW-COUNTER:FALSE
X-MICROSOFT-LOCATIONS:[]
BEGIN:VALARM
DESCRIPTION:REMINDER
TRIGGER;RELATED=START:-PT15M
ACTION:DISPLAY
END:VALARM
END:VEVENT
END:VCALENDAR
```


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="c0bdd-230">例 8: メッセージの会議出席依頼アイテムの添付ファイルの MIME 生の内容を取得する</span><span class="sxs-lookup"><span data-stu-id="c0bdd-230">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="c0bdd-231">要求</span><span class="sxs-lookup"><span data-stu-id="c0bdd-231">Request</span></span>

<span data-ttu-id="c0bdd-232">メッセージに添付されている会議出席依頼の生の内容 ( [eventmessage](../resources/eventmessage.md)型の) を取得する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-232">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="c0bdd-233">**Eventmessage**エンティティは、**メッセージ**の種類に基づいています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-233">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="c0bdd-234">応答</span><span class="sxs-lookup"><span data-stu-id="c0bdd-234">Response</span></span>
<span data-ttu-id="c0bdd-235">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-235">Here is an example of the response.</span></span> 

<span data-ttu-id="c0bdd-236">応答本文には、 **Eventmessage**添付ファイルが MIME 形式で含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-236">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="c0bdd-237">**イベントメッセージ**の本文は、簡潔にするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-237">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="c0bdd-238">完全なメッセージ本文は、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0bdd-238">The full message body is returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

From: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
To: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
Subject: Let's go for lunch
Thread-Topic: Let's go for lunch
Thread-Index: AdTPqxOmg4AXoJV960a1j5NrJCHYjA==
X-MS-Exchange-MessageSentRepresentingType: 1
Date: Thu, 28 Feb 2019 21:17:58 +0000
Message-ID:
    <CY4PR2201MB1046E9C83FC42478EF4EE283C9750@CY4PR2201MB1046.namprd22.prod.outlook.com>
Content-Language: en-US
X-MS-Has-Attach:
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
Content-Type: multipart/alternative;
    boundary="_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_"
MIME-Version: 1.0

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/plain; charset="us-ascii"

Does mid month work for you?

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/html; charset="us-ascii"

<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=us-ascii">
</head>
<body>
Does mid month work for you?
</body>
</html>

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/calendar; charset="utf-8"; method=REQUEST
Content-Transfer-Encoding: base64

QkVHSU46VkNBTEVOREFSDQpNRVRIT0Q6UkVRVUVTVA0KUFJPRElEOk1pY3Jvc29mdCBFeGNoYW5n


--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_--
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
  ]
}
-->
