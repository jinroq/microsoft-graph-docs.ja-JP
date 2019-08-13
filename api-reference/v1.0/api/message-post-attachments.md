---
title: 添付ファイルを追加する
description: '添付ファイルをメッセージに追加する場合に、この API を使用します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 476693776827df1e4d2ed20481ce6248a83496af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374724"
---
# <a name="add-attachment"></a><span data-ttu-id="c979b-103">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="c979b-103">Add attachment</span></span>

<span data-ttu-id="c979b-104">[添付ファイル](../resources/attachment.md)をメッセージに追加する場合に、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="c979b-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="c979b-105">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="c979b-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="c979b-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="c979b-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="c979b-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="c979b-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="c979b-108">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="c979b-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="c979b-109">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="c979b-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="c979b-110">既存のメッセージの添付ファイルのコレクションに投稿してそのメッセージに添付ファイルを追加したり、[作成してすぐ送信される](../api/user-sendmail.md)メッセージに添付ファイルを追加したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="c979b-110">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="c979b-111">現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="c979b-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="c979b-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c979b-112">Permissions</span></span>
<span data-ttu-id="c979b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c979b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c979b-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c979b-115">Permission type</span></span>      | <span data-ttu-id="c979b-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c979b-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c979b-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c979b-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c979b-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c979b-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c979b-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c979b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c979b-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c979b-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c979b-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c979b-121">Application</span></span> | <span data-ttu-id="c979b-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c979b-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c979b-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c979b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c979b-124">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="c979b-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="c979b-125">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="c979b-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="c979b-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="c979b-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c979b-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c979b-128">Request headers</span></span>
| <span data-ttu-id="c979b-129">名前</span><span class="sxs-lookup"><span data-stu-id="c979b-129">Name</span></span>       | <span data-ttu-id="c979b-130">型</span><span class="sxs-lookup"><span data-stu-id="c979b-130">Type</span></span> | <span data-ttu-id="c979b-131">説明</span><span class="sxs-lookup"><span data-stu-id="c979b-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c979b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="c979b-132">Authorization</span></span>  | <span data-ttu-id="c979b-133">string</span><span class="sxs-lookup"><span data-stu-id="c979b-133">string</span></span>  | <span data-ttu-id="c979b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c979b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c979b-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c979b-136">Content-Type</span></span> | <span data-ttu-id="c979b-137">string</span><span class="sxs-lookup"><span data-stu-id="c979b-137">string</span></span>  | <span data-ttu-id="c979b-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="c979b-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c979b-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="c979b-140">Request body</span></span>
<span data-ttu-id="c979b-141">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c979b-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c979b-142">応答</span><span class="sxs-lookup"><span data-stu-id="c979b-142">Response</span></span>

<span data-ttu-id="c979b-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c979b-143">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="c979b-144">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="c979b-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="c979b-145">要求</span><span class="sxs-lookup"><span data-stu-id="c979b-145">Request</span></span>
<span data-ttu-id="c979b-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c979b-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c979b-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c979b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "base64R0lGODdhEAYEAA7"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c979b-148">C#</span><span class="sxs-lookup"><span data-stu-id="c979b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c979b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c979b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c979b-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="c979b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c979b-151">Java</span><span class="sxs-lookup"><span data-stu-id="c979b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c979b-152">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c979b-152">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c979b-153">応答</span><span class="sxs-lookup"><span data-stu-id="c979b-153">Response</span></span>
<span data-ttu-id="c979b-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c979b-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP 201 Created
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
    "contentBytes": "base64R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="c979b-155">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="c979b-155">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="c979b-156">要求</span><span class="sxs-lookup"><span data-stu-id="c979b-156">Request</span></span>
<span data-ttu-id="c979b-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c979b-157">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->

```
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
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


##### <a name="response"></a><span data-ttu-id="c979b-158">応答</span><span class="sxs-lookup"><span data-stu-id="c979b-158">Response</span></span>
<span data-ttu-id="c979b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c979b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
