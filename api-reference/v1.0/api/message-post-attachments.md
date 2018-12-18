---
title: 添付ファイルを追加する
description: '添付ファイルをメッセージに追加する場合に、この API を使用します。 '
author: angelgolfer-ms
ms.openlocfilehash: 868ce046a37d027c675b005cef013892deffe2a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314617"
---
# <a name="add-attachment"></a><span data-ttu-id="5f97e-103">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="5f97e-103">Add attachment</span></span>

<span data-ttu-id="5f97e-104">[添付ファイル](../resources/attachment.md)をメッセージに追加する場合に、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="5f97e-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="5f97e-105">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="5f97e-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="5f97e-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="5f97e-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="5f97e-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="5f97e-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="5f97e-108">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="5f97e-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="5f97e-109">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="5f97e-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="5f97e-110">既存のメッセージの添付ファイルのコレクションに投稿してそのメッセージに添付ファイルを追加したり、[作成してすぐ送信される](../api/user-sendmail.md)メッセージに添付ファイルを追加したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="5f97e-110">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="5f97e-111">現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="5f97e-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f97e-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f97e-112">Permissions</span></span>
<span data-ttu-id="5f97e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f97e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f97e-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f97e-115">Permission type</span></span>      | <span data-ttu-id="5f97e-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f97e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f97e-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f97e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="5f97e-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f97e-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f97e-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f97e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f97e-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f97e-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f97e-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f97e-121">Application</span></span> | <span data-ttu-id="5f97e-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f97e-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f97e-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f97e-123">HTTP request</span></span>
<span data-ttu-id="5f97e-124"><!-- { "blockType": "ignored" } -->ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="5f97e-124"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="5f97e-125">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="5f97e-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="5f97e-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="5f97e-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5f97e-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f97e-128">Request headers</span></span>
| <span data-ttu-id="5f97e-129">名前</span><span class="sxs-lookup"><span data-stu-id="5f97e-129">Name</span></span>       | <span data-ttu-id="5f97e-130">種類</span><span class="sxs-lookup"><span data-stu-id="5f97e-130">Type</span></span> | <span data-ttu-id="5f97e-131">説明</span><span class="sxs-lookup"><span data-stu-id="5f97e-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f97e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f97e-132">Authorization</span></span>  | <span data-ttu-id="5f97e-133">string</span><span class="sxs-lookup"><span data-stu-id="5f97e-133">string</span></span>  | <span data-ttu-id="5f97e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5f97e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f97e-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f97e-136">Content-Type</span></span> | <span data-ttu-id="5f97e-137">string</span><span class="sxs-lookup"><span data-stu-id="5f97e-137">string</span></span>  | <span data-ttu-id="5f97e-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="5f97e-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f97e-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f97e-140">Request body</span></span>
<span data-ttu-id="5f97e-141">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f97e-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5f97e-142">応答</span><span class="sxs-lookup"><span data-stu-id="5f97e-142">Response</span></span>

<span data-ttu-id="5f97e-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5f97e-143">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="5f97e-144">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="5f97e-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5f97e-145">要求</span><span class="sxs-lookup"><span data-stu-id="5f97e-145">Request</span></span>
<span data-ttu-id="5f97e-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f97e-146">Here is an example of the request.</span></span>
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

<span data-ttu-id="5f97e-147">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f97e-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5f97e-148">応答</span><span class="sxs-lookup"><span data-stu-id="5f97e-148">Response</span></span>
<span data-ttu-id="5f97e-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5f97e-149">Here is an example of the response.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="5f97e-150">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="5f97e-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5f97e-151">要求</span><span class="sxs-lookup"><span data-stu-id="5f97e-151">Request</span></span>
<span data-ttu-id="5f97e-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f97e-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_item_attachment_from_message"
}-->

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

##### <a name="response"></a><span data-ttu-id="5f97e-153">応答</span><span class="sxs-lookup"><span data-stu-id="5f97e-153">Response</span></span>
<span data-ttu-id="5f97e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f97e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
