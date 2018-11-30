---
title: 添付ファイルを追加する
description: 投稿に添付ファイルを追加するのにには、この API を使用します。 そこから
ms.openlocfilehash: 38126f015d19890a9a1f08d458f05505faa09e9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067721"
---
# <a name="add-attachment"></a><span data-ttu-id="e92cc-104">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="e92cc-104">Add attachment</span></span>

> <span data-ttu-id="e92cc-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e92cc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e92cc-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e92cc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e92cc-p103">[添付ファイル](../resources/attachment.md)を投稿に追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="e92cc-p103">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="e92cc-109">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="e92cc-109">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="e92cc-110">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="e92cc-110">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="e92cc-111">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="e92cc-111">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="e92cc-112">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="e92cc-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="e92cc-113">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="e92cc-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e92cc-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e92cc-114">Permissions</span></span>
<span data-ttu-id="e92cc-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e92cc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e92cc-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e92cc-117">Permission type</span></span>      | <span data-ttu-id="e92cc-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e92cc-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e92cc-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e92cc-119">Delegated (work or school account)</span></span> | <span data-ttu-id="e92cc-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e92cc-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e92cc-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e92cc-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e92cc-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e92cc-122">Not supported.</span></span>    |
|<span data-ttu-id="e92cc-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e92cc-123">Application</span></span> | <span data-ttu-id="e92cc-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e92cc-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e92cc-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e92cc-125">HTTP request</span></span>
<span data-ttu-id="e92cc-126"><!-- { "blockType": "ignored" } -->[転記](../resources/post.md)グループの[会話](../resources/conversation.md)に属している[スレッド](../resources/conversationthread.md)での添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="e92cc-126"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="e92cc-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e92cc-127">Request headers</span></span>
| <span data-ttu-id="e92cc-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e92cc-128">Header</span></span>       | <span data-ttu-id="e92cc-129">値</span><span class="sxs-lookup"><span data-stu-id="e92cc-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e92cc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e92cc-130">Authorization</span></span>  | <span data-ttu-id="e92cc-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e92cc-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e92cc-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="e92cc-133">Request body</span></span>
<span data-ttu-id="e92cc-134">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e92cc-134">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e92cc-135">応答</span><span class="sxs-lookup"><span data-stu-id="e92cc-135">Response</span></span>

<span data-ttu-id="e92cc-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e92cc-136">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="e92cc-137">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="e92cc-137">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e92cc-138">要求</span><span class="sxs-lookup"><span data-stu-id="e92cc-138">Request</span></span>
<span data-ttu-id="e92cc-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e92cc-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="e92cc-140">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e92cc-140">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="e92cc-141">応答</span><span class="sxs-lookup"><span data-stu-id="e92cc-141">Response</span></span>
<span data-ttu-id="e92cc-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e92cc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="e92cc-145">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="e92cc-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e92cc-146">要求</span><span class="sxs-lookup"><span data-stu-id="e92cc-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="e92cc-147">応答</span><span class="sxs-lookup"><span data-stu-id="e92cc-147">Response</span></span>
<span data-ttu-id="e92cc-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e92cc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


## <a name="example-reference-attachment"></a><span data-ttu-id="e92cc-151">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="e92cc-151">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e92cc-152">要求</span><span class="sxs-lookup"><span data-stu-id="e92cc-152">Request</span></span>
<span data-ttu-id="e92cc-153">ここでは、既存の投稿の添付ファイル、参照を追加する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e92cc-153">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="e92cc-154">添付ファイルは、OneDrive 上のフォルダーをポイントします。</span><span class="sxs-lookup"><span data-stu-id="e92cc-154">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_post",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments
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

##### <a name="response"></a><span data-ttu-id="e92cc-155">応答</span><span class="sxs-lookup"><span data-stu-id="e92cc-155">Response</span></span>
<span data-ttu-id="e92cc-156">ここでは、完全な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e92cc-156">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments/$entity",
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
