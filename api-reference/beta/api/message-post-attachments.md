---
title: 添付ファイルを追加する
description: '添付ファイルをメッセージに追加する場合に、この API を使用します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9457aa138068b3059b1fabbd606268f6e756b94e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862770"
---
# <a name="add-attachment"></a><span data-ttu-id="6c8b5-103">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="6c8b5-103">Add attachment</span></span>

> <span data-ttu-id="6c8b5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c8b5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c8b5-106">[添付ファイル](../resources/attachment.md)をメッセージに追加する場合に、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-106">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="6c8b5-107">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="6c8b5-108">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="6c8b5-109">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="6c8b5-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="6c8b5-111">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="6c8b5-112">既存のメッセージに添付ファイルを追加するには、添付ファイルのコレクションへの投稿または新しいメッセージをされている[ドラフト](../api/user-post-messages.md)、または[作成され実行時に送信](../api/user-sendmail.md)します。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-112">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="6c8b5-113">現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-113">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c8b5-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c8b5-114">Permissions</span></span>
<span data-ttu-id="6c8b5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c8b5-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c8b5-117">Permission type</span></span>      | <span data-ttu-id="6c8b5-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c8b5-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c8b5-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c8b5-119">Delegated (work or school account)</span></span> | <span data-ttu-id="6c8b5-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c8b5-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6c8b5-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c8b5-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c8b5-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c8b5-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6c8b5-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c8b5-123">Application</span></span> | <span data-ttu-id="6c8b5-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c8b5-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c8b5-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c8b5-125">HTTP request</span></span>
<span data-ttu-id="6c8b5-126"><!-- { "blockType": "ignored" } -->ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-126"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="6c8b5-127">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-127">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="6c8b5-p103">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6c8b5-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c8b5-130">Request headers</span></span>
| <span data-ttu-id="6c8b5-131">名前</span><span class="sxs-lookup"><span data-stu-id="6c8b5-131">Name</span></span>       | <span data-ttu-id="6c8b5-132">種類</span><span class="sxs-lookup"><span data-stu-id="6c8b5-132">Type</span></span> | <span data-ttu-id="6c8b5-133">説明</span><span class="sxs-lookup"><span data-stu-id="6c8b5-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c8b5-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c8b5-134">Authorization</span></span>  | <span data-ttu-id="6c8b5-135">string</span><span class="sxs-lookup"><span data-stu-id="6c8b5-135">string</span></span>  | <span data-ttu-id="6c8b5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c8b5-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c8b5-138">Content-Type</span></span> | <span data-ttu-id="6c8b5-139">string</span><span class="sxs-lookup"><span data-stu-id="6c8b5-139">string</span></span>  | <span data-ttu-id="6c8b5-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c8b5-142">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c8b5-142">Request body</span></span>
<span data-ttu-id="6c8b5-143">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-143">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6c8b5-144">応答</span><span class="sxs-lookup"><span data-stu-id="6c8b5-144">Response</span></span>

<span data-ttu-id="6c8b5-145">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文の[添付](../resources/attachment.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-145">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="6c8b5-146">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="6c8b5-146">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="6c8b5-147">要求</span><span class="sxs-lookup"><span data-stu-id="6c8b5-147">Request</span></span>
<span data-ttu-id="6c8b5-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="6c8b5-149">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-149">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6c8b5-150">応答</span><span class="sxs-lookup"><span data-stu-id="6c8b5-150">Response</span></span>
<span data-ttu-id="6c8b5-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 202

{
    "id": "AAMkADNkN2R",
    "lastModifiedDateTime": "2017-01-26T08:48:28Z",
    "name": "smile",
    "contentType": "image/gif",
    "size": 1008,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "R0lGODdhEAYEAA7"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="6c8b5-152">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="6c8b5-152">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="6c8b5-153">要求</span><span class="sxs-lookup"><span data-stu-id="6c8b5-153">Request</span></span>
<span data-ttu-id="6c8b5-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
    "@odata.type": "microsoft.graph.event",
    "subject": "Discuss gifts for children",
    "body": {
      "contentType": "HTML",
      "content": "Let's look for funding!"
    },
    "start": {
      "dateTime": "2016-12-02T18:00:00",
      "timeZone": "Pacific Standard Time"
    },
    "end": {
      "dateTime": "2016-12-02T19:00:00",
      "timeZone": "Pacific Standard Time"
    }
  }
}

```

##### <a name="response"></a><span data-ttu-id="6c8b5-155">応答</span><span class="sxs-lookup"><span data-stu-id="6c8b5-155">Response</span></span>
<span data-ttu-id="6c8b5-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "id":"AAMkADNkNJp5JVnQIe9r0=",
  "lastModifiedDateTime":"2016-12-01T22:27:13Z",
  "name":"Holiday event",
  "contentType":null,
  "size":2473,
  "isInline":false
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="6c8b5-159">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="6c8b5-159">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="6c8b5-160">要求</span><span class="sxs-lookup"><span data-stu-id="6c8b5-160">Request</span></span>
<span data-ttu-id="6c8b5-161">ここでは、既存のメッセージの添付ファイル、参照を追加する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-161">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="6c8b5-162">添付ファイルは、OneDrive 上のフォルダーをポイントします。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-162">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_message",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M88AADUv0uFAAA=/attachments
Content-type: application/json
Content-length: 319

{ 
    "@odata.type": "#microsoft.graph.referenceAttachment", 
    "name": "Personal pictures", 
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    "providerType": "oneDriveConsumer", 
    "permission": "Edit", 
    "isFolder": "True" 
} 
```

##### <a name="response"></a><span data-ttu-id="6c8b5-163">応答</span><span class="sxs-lookup"><span data-stu-id="6c8b5-163">Response</span></span>
<span data-ttu-id="6c8b5-164">ここでは、完全な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6c8b5-164">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/messages/AAMkAGE1M88AADUv0uFAAA%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PICVGCc0g=",
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
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
