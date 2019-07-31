---
title: 添付ファイルを追加する
description: '添付ファイルをメッセージに追加する場合に、この API を使用します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2f420bef7085bc91089f92efc2bc910f3a14b436
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983860"
---
# <a name="add-attachment"></a><span data-ttu-id="9ed0c-103">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="9ed0c-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ed0c-104">[添付ファイル](../resources/attachment.md)をメッセージに追加する場合に、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="9ed0c-105">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="9ed0c-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="9ed0c-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="9ed0c-108">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="9ed0c-109">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="9ed0c-110">添付ファイルを既存のメッセージに追加するには、添付ファイルのコレクションに投稿するか、[ドラフト](../api/user-post-messages.md)されている新しいメッセージに投稿するか、その[場で作成して送信](../api/user-sendmail.md)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-110">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="9ed0c-111">現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ed0c-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ed0c-112">Permissions</span></span>
<span data-ttu-id="9ed0c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed0c-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ed0c-115">Permission type</span></span>      | <span data-ttu-id="9ed0c-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ed0c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ed0c-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ed0c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="9ed0c-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed0c-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9ed0c-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ed0c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed0c-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed0c-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9ed0c-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ed0c-121">Application</span></span> | <span data-ttu-id="9ed0c-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed0c-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ed0c-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ed0c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9ed0c-124">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="9ed0c-125">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="9ed0c-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9ed0c-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ed0c-128">Request headers</span></span>
| <span data-ttu-id="9ed0c-129">名前</span><span class="sxs-lookup"><span data-stu-id="9ed0c-129">Name</span></span>       | <span data-ttu-id="9ed0c-130">型</span><span class="sxs-lookup"><span data-stu-id="9ed0c-130">Type</span></span> | <span data-ttu-id="9ed0c-131">説明</span><span class="sxs-lookup"><span data-stu-id="9ed0c-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ed0c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed0c-132">Authorization</span></span>  | <span data-ttu-id="9ed0c-133">string</span><span class="sxs-lookup"><span data-stu-id="9ed0c-133">string</span></span>  | <span data-ttu-id="9ed0c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ed0c-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ed0c-136">Content-Type</span></span> | <span data-ttu-id="9ed0c-137">string</span><span class="sxs-lookup"><span data-stu-id="9ed0c-137">string</span></span>  | <span data-ttu-id="9ed0c-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ed0c-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ed0c-140">Request body</span></span>
<span data-ttu-id="9ed0c-141">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9ed0c-142">応答</span><span class="sxs-lookup"><span data-stu-id="9ed0c-142">Response</span></span>

<span data-ttu-id="9ed0c-143">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[Attachment](../resources/attachment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-143">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="9ed0c-144">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="9ed0c-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9ed0c-145">要求</span><span class="sxs-lookup"><span data-stu-id="9ed0c-145">Request</span></span>
<span data-ttu-id="9ed0c-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ed0c-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9ed0c-147">HTTP</span></span>](#tab/http)
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
  "contentBytes": "a0b1c76de9f7="
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ed0c-148">C#</span><span class="sxs-lookup"><span data-stu-id="9ed0c-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ed0c-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ed0c-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ed0c-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="9ed0c-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9ed0c-151">Java</span><span class="sxs-lookup"><span data-stu-id="9ed0c-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="9ed0c-152">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-152">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9ed0c-153">応答</span><span class="sxs-lookup"><span data-stu-id="9ed0c-153">Response</span></span>
<span data-ttu-id="9ed0c-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-154">Here is an example of the response.</span></span> 
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
    "contentBytes": "a0b1c76de9f7="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="9ed0c-155">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="9ed0c-155">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9ed0c-156">要求</span><span class="sxs-lookup"><span data-stu-id="9ed0c-156">Request</span></span>
<span data-ttu-id="9ed0c-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-157">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->

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


##### <a name="response"></a><span data-ttu-id="9ed0c-158">応答</span><span class="sxs-lookup"><span data-stu-id="9ed0c-158">Response</span></span>
<span data-ttu-id="9ed0c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="9ed0c-162">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="9ed0c-162">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9ed0c-163">要求</span><span class="sxs-lookup"><span data-stu-id="9ed0c-163">Request</span></span>
<span data-ttu-id="9ed0c-164">既存のメッセージに参照添付ファイルを追加する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-164">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="9ed0c-165">添付ファイルは、OneDrive 上のフォルダーを指します。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-165">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ed0c-166">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9ed0c-166">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ed0c-167">C#</span><span class="sxs-lookup"><span data-stu-id="9ed0c-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ed0c-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ed0c-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ed0c-169">目的-C</span><span class="sxs-lookup"><span data-stu-id="9ed0c-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9ed0c-170">Java</span><span class="sxs-lookup"><span data-stu-id="9ed0c-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-from-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ed0c-171">応答</span><span class="sxs-lookup"><span data-stu-id="9ed0c-171">Response</span></span>
<span data-ttu-id="9ed0c-172">完全な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ed0c-172">Here is an example of a full response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_file_attachment_from_message/contentBytes:\r\n      Expected type Binary but actual was String. Property: contentBytes, actual value: 'a0b1c76de9f7='"
  ]
}
-->
