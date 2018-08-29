# <a name="add-attachment"></a><span data-ttu-id="f76bc-101">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="f76bc-101">Add attachment</span></span>

<span data-ttu-id="f76bc-102">この API を使用して、新しい添付ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="f76bc-102">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="f76bc-103">添付ファイルは、次の種類のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="f76bc-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="f76bc-104">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="f76bc-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="f76bc-105">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、メッセージ)。</span><span class="sxs-lookup"><span data-stu-id="f76bc-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="f76bc-106">ファイルへのリンク ([referenceAttachment](../resources/referenceAttachment.md) リソース)。</span><span class="sxs-lookup"><span data-stu-id="f76bc-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="f76bc-107">これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="f76bc-107">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f76bc-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f76bc-108">Permissions</span></span>
<span data-ttu-id="f76bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f76bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f76bc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f76bc-111">Permission type</span></span>      | <span data-ttu-id="f76bc-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f76bc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f76bc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f76bc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f76bc-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f76bc-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f76bc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f76bc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f76bc-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f76bc-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f76bc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f76bc-117">Application</span></span> | <span data-ttu-id="f76bc-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f76bc-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f76bc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f76bc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="f76bc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f76bc-120">Request headers</span></span>
| <span data-ttu-id="f76bc-121">名前</span><span class="sxs-lookup"><span data-stu-id="f76bc-121">Name</span></span>       | <span data-ttu-id="f76bc-122">型</span><span class="sxs-lookup"><span data-stu-id="f76bc-122">Type</span></span> | <span data-ttu-id="f76bc-123">説明</span><span class="sxs-lookup"><span data-stu-id="f76bc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f76bc-124">承認</span><span class="sxs-lookup"><span data-stu-id="f76bc-124">Authorization</span></span>  | <span data-ttu-id="f76bc-125">文字列</span><span class="sxs-lookup"><span data-stu-id="f76bc-125">string</span></span>  | <span data-ttu-id="f76bc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f76bc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f76bc-128">コンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="f76bc-128">Content-Type</span></span> | <span data-ttu-id="f76bc-129">文字列</span><span class="sxs-lookup"><span data-stu-id="f76bc-129">string</span></span>  | <span data-ttu-id="f76bc-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="f76bc-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f76bc-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="f76bc-132">Request body</span></span>
<span data-ttu-id="f76bc-133">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f76bc-133">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f76bc-134">応答</span><span class="sxs-lookup"><span data-stu-id="f76bc-134">Response</span></span>

<span data-ttu-id="f76bc-135">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f76bc-135">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f76bc-136">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="f76bc-136">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="f76bc-137">要求</span><span class="sxs-lookup"><span data-stu-id="f76bc-137">Request</span></span>
<span data-ttu-id="f76bc-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f76bc-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="f76bc-139">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f76bc-139">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f76bc-140">応答</span><span class="sxs-lookup"><span data-stu-id="f76bc-140">Response</span></span>
<span data-ttu-id="f76bc-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f76bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="f76bc-144">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="f76bc-144">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f76bc-145">要求</span><span class="sxs-lookup"><span data-stu-id="f76bc-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="f76bc-146">応答</span><span class="sxs-lookup"><span data-stu-id="f76bc-146">Response</span></span>
<span data-ttu-id="f76bc-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f76bc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
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
