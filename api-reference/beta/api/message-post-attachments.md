---
title: 添付ファイルを追加する
description: '添付ファイルをメッセージに追加する場合に、この API を使用します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c2d6c0724334103691648f0792282ff8c67b906d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266060"
---
# <a name="add-attachment"></a><span data-ttu-id="eea78-103">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="eea78-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eea78-104">[添付ファイル](../resources/attachment.md)をメッセージに追加する場合に、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="eea78-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="eea78-105">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="eea78-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="eea78-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="eea78-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="eea78-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="eea78-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="eea78-108">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="eea78-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="eea78-109">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="eea78-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="eea78-110">添付ファイルを既存のメッセージに追加するには、添付ファイルのコレクションに投稿するか、[ドラフト](../api/user-post-messages.md)されている新しいメッセージに投稿するか、その[場で作成して送信](../api/user-sendmail.md)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="eea78-110">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="eea78-111">現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="eea78-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="eea78-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eea78-112">Permissions</span></span>
<span data-ttu-id="eea78-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eea78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eea78-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eea78-115">Permission type</span></span>      | <span data-ttu-id="eea78-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eea78-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eea78-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eea78-117">Delegated (work or school account)</span></span> | <span data-ttu-id="eea78-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eea78-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eea78-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eea78-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eea78-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eea78-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eea78-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eea78-121">Application</span></span> | <span data-ttu-id="eea78-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eea78-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eea78-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eea78-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="eea78-124">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="eea78-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="eea78-125">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="eea78-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="eea78-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="eea78-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eea78-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eea78-128">Request headers</span></span>
| <span data-ttu-id="eea78-129">名前</span><span class="sxs-lookup"><span data-stu-id="eea78-129">Name</span></span>       | <span data-ttu-id="eea78-130">型</span><span class="sxs-lookup"><span data-stu-id="eea78-130">Type</span></span> | <span data-ttu-id="eea78-131">説明</span><span class="sxs-lookup"><span data-stu-id="eea78-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eea78-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="eea78-132">Authorization</span></span>  | <span data-ttu-id="eea78-133">string</span><span class="sxs-lookup"><span data-stu-id="eea78-133">string</span></span>  | <span data-ttu-id="eea78-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eea78-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eea78-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eea78-136">Content-Type</span></span> | <span data-ttu-id="eea78-137">string</span><span class="sxs-lookup"><span data-stu-id="eea78-137">string</span></span>  | <span data-ttu-id="eea78-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="eea78-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eea78-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="eea78-140">Request body</span></span>
<span data-ttu-id="eea78-141">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eea78-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eea78-142">応答</span><span class="sxs-lookup"><span data-stu-id="eea78-142">Response</span></span>

<span data-ttu-id="eea78-143">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[Attachment](../resources/attachment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eea78-143">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="eea78-144">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="eea78-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="eea78-145">要求</span><span class="sxs-lookup"><span data-stu-id="eea78-145">Request</span></span>
<span data-ttu-id="eea78-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eea78-146">Here is an example of the request.</span></span>
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

<span data-ttu-id="eea78-147">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eea78-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eea78-148">応答</span><span class="sxs-lookup"><span data-stu-id="eea78-148">Response</span></span>
<span data-ttu-id="eea78-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="eea78-149">Here is an example of the response.</span></span> 
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="eea78-150">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="eea78-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eea78-151">C#</span><span class="sxs-lookup"><span data-stu-id="eea78-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eea78-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="eea78-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eea78-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="eea78-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="eea78-154">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="eea78-154">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="eea78-155">要求</span><span class="sxs-lookup"><span data-stu-id="eea78-155">Request</span></span>
<span data-ttu-id="eea78-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eea78-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eea78-157">応答</span><span class="sxs-lookup"><span data-stu-id="eea78-157">Response</span></span>
<span data-ttu-id="eea78-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eea78-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="eea78-161">例 (添付ファイルの参照)</span><span class="sxs-lookup"><span data-stu-id="eea78-161">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="eea78-162">要求</span><span class="sxs-lookup"><span data-stu-id="eea78-162">Request</span></span>
<span data-ttu-id="eea78-163">既存のメッセージに参照添付ファイルを追加する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eea78-163">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="eea78-164">添付ファイルは、OneDrive 上のフォルダーを指します。</span><span class="sxs-lookup"><span data-stu-id="eea78-164">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eea78-165">応答</span><span class="sxs-lookup"><span data-stu-id="eea78-165">Response</span></span>
<span data-ttu-id="eea78-166">完全な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eea78-166">Here is an example of a full response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="eea78-167">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="eea78-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eea78-168">C#</span><span class="sxs-lookup"><span data-stu-id="eea78-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eea78-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="eea78-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eea78-170">目的-C</span><span class="sxs-lookup"><span data-stu-id="eea78-170">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_message-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


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
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: create_file_attachment_from_message/contentBytes:\r\n      Expected type Binary but actual was String. Property: contentBytes, actual value: 'a0b1c76de9f7='"
  ]
}
-->
