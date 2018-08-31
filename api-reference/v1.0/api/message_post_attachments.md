# <a name="add-attachment"></a><span data-ttu-id="42cb8-101">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="42cb8-101">Add attachment</span></span>

<span data-ttu-id="42cb8-102">[添付ファイル](../resources/attachment.md)をメッセージに追加する場合に、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="42cb8-102">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="42cb8-103">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="42cb8-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="42cb8-104">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="42cb8-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="42cb8-105">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="42cb8-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="42cb8-106">ファイルへのリンク ([referenceAttachment](../resources/referenceAttachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="42cb8-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="42cb8-107">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="42cb8-107">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="42cb8-108">既存のメッセージの添付ファイルのコレクションに投稿してそのメッセージに添付ファイルを追加したり、[作成してすぐ送信される](../api/user_sendmail.md)メッセージに添付ファイルを追加したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="42cb8-108">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user_sendmail.md).</span></span>

<span data-ttu-id="42cb8-109">現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="42cb8-109">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="42cb8-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="42cb8-110">Permissions</span></span>
<span data-ttu-id="42cb8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42cb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="42cb8-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42cb8-113">Permission type</span></span>      | <span data-ttu-id="42cb8-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="42cb8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42cb8-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="42cb8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="42cb8-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42cb8-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="42cb8-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42cb8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42cb8-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42cb8-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="42cb8-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42cb8-119">Application</span></span> | <span data-ttu-id="42cb8-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42cb8-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="42cb8-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42cb8-121">HTTP request</span></span>
<span data-ttu-id="42cb8-122"><!-- { "blockType": "ignored" } --> ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="42cb8-122">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="42cb8-123">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="42cb8-123">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="42cb8-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="42cb8-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="42cb8-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42cb8-126">Request headers</span></span>
| <span data-ttu-id="42cb8-127">名前</span><span class="sxs-lookup"><span data-stu-id="42cb8-127">Name</span></span>       | <span data-ttu-id="42cb8-128">型</span><span class="sxs-lookup"><span data-stu-id="42cb8-128">Type</span></span> | <span data-ttu-id="42cb8-129">説明</span><span class="sxs-lookup"><span data-stu-id="42cb8-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42cb8-130">承認</span><span class="sxs-lookup"><span data-stu-id="42cb8-130">Authorization</span></span>  | <span data-ttu-id="42cb8-131">文字列</span><span class="sxs-lookup"><span data-stu-id="42cb8-131">string</span></span>  | <span data-ttu-id="42cb8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="42cb8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42cb8-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42cb8-134">Content-Type</span></span> | <span data-ttu-id="42cb8-135">string</span><span class="sxs-lookup"><span data-stu-id="42cb8-135">string</span></span>  | <span data-ttu-id="42cb8-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="42cb8-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42cb8-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="42cb8-138">Request body</span></span>
<span data-ttu-id="42cb8-139">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="42cb8-139">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="42cb8-140">応答</span><span class="sxs-lookup"><span data-stu-id="42cb8-140">Response</span></span>

<span data-ttu-id="42cb8-141">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="42cb8-141">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="42cb8-142">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="42cb8-142">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="42cb8-143">要求</span><span class="sxs-lookup"><span data-stu-id="42cb8-143">Request</span></span>
<span data-ttu-id="42cb8-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="42cb8-144">Here is an example of the request.</span></span>
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

<span data-ttu-id="42cb8-145">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="42cb8-145">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="42cb8-146">応答</span><span class="sxs-lookup"><span data-stu-id="42cb8-146">Response</span></span>
<span data-ttu-id="42cb8-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="42cb8-147">Here is an example of the response.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="42cb8-148">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="42cb8-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="42cb8-149">要求</span><span class="sxs-lookup"><span data-stu-id="42cb8-149">Request</span></span>
<span data-ttu-id="42cb8-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="42cb8-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="42cb8-151">応答</span><span class="sxs-lookup"><span data-stu-id="42cb8-151">Response</span></span>
<span data-ttu-id="42cb8-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="42cb8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
