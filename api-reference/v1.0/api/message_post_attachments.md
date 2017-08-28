# <a name="add-attachment"></a><span data-ttu-id="e05c3-101">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="e05c3-101">Add attachment</span></span>

<span data-ttu-id="e05c3-102">[添付ファイル](../resources/attachment.md)をメッセージに追加する場合に、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="e05c3-102">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="e05c3-103">既存のメッセージの添付ファイルのコレクションに投稿してそのメッセージに添付ファイルを追加したり、[作成してすぐ送信される](../api/user_sendmail.md)メッセージに添付ファイルを追加したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="e05c3-103">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user_sendmail.md).</span></span>

<span data-ttu-id="e05c3-104">現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="e05c3-104">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="e05c3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e05c3-105">Permissions</span></span>
<span data-ttu-id="e05c3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e05c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e05c3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e05c3-108">Permission type</span></span>      | <span data-ttu-id="e05c3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e05c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e05c3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e05c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e05c3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e05c3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e05c3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e05c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e05c3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e05c3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e05c3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e05c3-114">Application</span></span> | <span data-ttu-id="e05c3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e05c3-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e05c3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e05c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e05c3-117">ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="e05c3-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="e05c3-118">ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="e05c3-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="e05c3-p102">ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="e05c3-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e05c3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e05c3-121">Request headers</span></span>
| <span data-ttu-id="e05c3-122">名前</span><span class="sxs-lookup"><span data-stu-id="e05c3-122">Name</span></span>       | <span data-ttu-id="e05c3-123">型</span><span class="sxs-lookup"><span data-stu-id="e05c3-123">Type</span></span> | <span data-ttu-id="e05c3-124">説明</span><span class="sxs-lookup"><span data-stu-id="e05c3-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e05c3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e05c3-125">Authorization</span></span>  | <span data-ttu-id="e05c3-126">string</span><span class="sxs-lookup"><span data-stu-id="e05c3-126">string</span></span>  | <span data-ttu-id="e05c3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e05c3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e05c3-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e05c3-129">Content-Type</span></span> | <span data-ttu-id="e05c3-130">string</span><span class="sxs-lookup"><span data-stu-id="e05c3-130">string</span></span>  | <span data-ttu-id="e05c3-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="e05c3-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e05c3-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="e05c3-133">Request body</span></span>
<span data-ttu-id="e05c3-134">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e05c3-134">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e05c3-135">応答</span><span class="sxs-lookup"><span data-stu-id="e05c3-135">Response</span></span>

<span data-ttu-id="e05c3-136">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e05c3-136">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="e05c3-137">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="e05c3-137">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e05c3-138">要求</span><span class="sxs-lookup"><span data-stu-id="e05c3-138">Request</span></span>
<span data-ttu-id="e05c3-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e05c3-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="e05c3-140">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e05c3-140">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e05c3-141">応答</span><span class="sxs-lookup"><span data-stu-id="e05c3-141">Response</span></span>
<span data-ttu-id="e05c3-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e05c3-142">Here is an example of the response.</span></span>
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
    "contentBytes": "R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="e05c3-143">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="e05c3-143">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e05c3-144">要求</span><span class="sxs-lookup"><span data-stu-id="e05c3-144">Request</span></span>
<span data-ttu-id="e05c3-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e05c3-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
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

##### <a name="response"></a><span data-ttu-id="e05c3-146">応答</span><span class="sxs-lookup"><span data-stu-id="e05c3-146">Response</span></span>
<span data-ttu-id="e05c3-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e05c3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
