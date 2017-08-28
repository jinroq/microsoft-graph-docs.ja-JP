# <a name="add-attachment"></a><span data-ttu-id="17683-101">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="17683-101">Add attachment</span></span>

<span data-ttu-id="17683-102">この API を使用して、新しい添付ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="17683-102">Use this API to create a new Attachment.</span></span>
## <a name="permissions"></a><span data-ttu-id="17683-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="17683-103">Permissions</span></span>
<span data-ttu-id="17683-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="17683-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="17683-106">Permission type</span></span>      | <span data-ttu-id="17683-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="17683-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17683-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="17683-108">Delegated (work or school account)</span></span> | <span data-ttu-id="17683-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17683-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="17683-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="17683-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17683-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17683-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="17683-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="17683-112">Application</span></span> | <span data-ttu-id="17683-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17683-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="17683-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17683-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="17683-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17683-115">Request headers</span></span>
| <span data-ttu-id="17683-116">名前</span><span class="sxs-lookup"><span data-stu-id="17683-116">Name</span></span>       | <span data-ttu-id="17683-117">型</span><span class="sxs-lookup"><span data-stu-id="17683-117">Type</span></span> | <span data-ttu-id="17683-118">説明</span><span class="sxs-lookup"><span data-stu-id="17683-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="17683-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="17683-119">Authorization</span></span>  | <span data-ttu-id="17683-120">string</span><span class="sxs-lookup"><span data-stu-id="17683-120">string</span></span>  | <span data-ttu-id="17683-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="17683-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17683-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17683-123">Content-Type</span></span> | <span data-ttu-id="17683-124">string</span><span class="sxs-lookup"><span data-stu-id="17683-124">string</span></span>  | <span data-ttu-id="17683-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="17683-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17683-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="17683-127">Request body</span></span>
<span data-ttu-id="17683-128">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="17683-128">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="17683-129">応答</span><span class="sxs-lookup"><span data-stu-id="17683-129">Response</span></span>

<span data-ttu-id="17683-130">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="17683-130">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="17683-131">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="17683-131">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="17683-132">要求</span><span class="sxs-lookup"><span data-stu-id="17683-132">Request</span></span>
<span data-ttu-id="17683-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="17683-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="17683-134">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="17683-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="17683-135">応答</span><span class="sxs-lookup"><span data-stu-id="17683-135">Response</span></span>
<span data-ttu-id="17683-p104">以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="17683-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="17683-139">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="17683-139">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="17683-140">要求</span><span class="sxs-lookup"><span data-stu-id="17683-140">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="17683-141">応答</span><span class="sxs-lookup"><span data-stu-id="17683-141">Response</span></span>
<span data-ttu-id="17683-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="17683-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
