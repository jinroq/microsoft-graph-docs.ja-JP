# <a name="fileattachment-resource-type"></a><span data-ttu-id="2c923-101">fileAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c923-101">fileAttachment resource type</span></span>

<span data-ttu-id="2c923-p101">イベント、メッセージまたは投稿に添付されたファイル (テキスト ファイルや Word 文書など) です。**contentBytes** プロパティには、base64 でエンコードされたファイルの内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2c923-p101">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="2c923-104">添付ファイルを作成する場合は、要求本文に以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2c923-104">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="2c923-105">必要なプロパティ **name** と **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="2c923-105">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="2c923-106">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="2c923-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2c923-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c923-107">Methods</span></span>

| <span data-ttu-id="2c923-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c923-108">Method</span></span>       | <span data-ttu-id="2c923-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2c923-109">Return Type</span></span>  |<span data-ttu-id="2c923-110">説明</span><span class="sxs-lookup"><span data-stu-id="2c923-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c923-111">取得</span><span class="sxs-lookup"><span data-stu-id="2c923-111">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="2c923-112">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="2c923-112">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="2c923-113">fileattachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2c923-113">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="2c923-114">削除</span><span class="sxs-lookup"><span data-stu-id="2c923-114">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="2c923-115">なし</span><span class="sxs-lookup"><span data-stu-id="2c923-115">None</span></span> |<span data-ttu-id="2c923-116">fileAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2c923-116">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2c923-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c923-117">Properties</span></span>
| <span data-ttu-id="2c923-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c923-118">Property</span></span>     | <span data-ttu-id="2c923-119">タイプ</span><span class="sxs-lookup"><span data-stu-id="2c923-119">Type</span></span>   |<span data-ttu-id="2c923-120">説明</span><span class="sxs-lookup"><span data-stu-id="2c923-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c923-121">contentBytes</span><span class="sxs-lookup"><span data-stu-id="2c923-121">contentBytes</span></span>|<span data-ttu-id="2c923-122">バイナリ</span><span class="sxs-lookup"><span data-stu-id="2c923-122">Binary</span></span>|<span data-ttu-id="2c923-123">base64 でエンコードされたファイルの内容。</span><span class="sxs-lookup"><span data-stu-id="2c923-123">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="2c923-124">contentId</span><span class="sxs-lookup"><span data-stu-id="2c923-124">contentId</span></span>|<span data-ttu-id="2c923-125">文字列</span><span class="sxs-lookup"><span data-stu-id="2c923-125">String</span></span>|<span data-ttu-id="2c923-126">Exchange ストア内の添付ファイルの ID。</span><span class="sxs-lookup"><span data-stu-id="2c923-126">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="2c923-127">contentLocation</span><span class="sxs-lookup"><span data-stu-id="2c923-127">contentLocation</span></span>|<span data-ttu-id="2c923-128">文字列</span><span class="sxs-lookup"><span data-stu-id="2c923-128">String</span></span>|<span data-ttu-id="2c923-129">添付ファイルのコンテンツの場所に対応する Uniform Resource Identifier (URI)。</span><span class="sxs-lookup"><span data-stu-id="2c923-129">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="2c923-130">contentType</span><span class="sxs-lookup"><span data-stu-id="2c923-130">contentType</span></span>|<span data-ttu-id="2c923-131">文字列</span><span class="sxs-lookup"><span data-stu-id="2c923-131">String</span></span>|<span data-ttu-id="2c923-132">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="2c923-132">The content type of the attachment.</span></span>|
|<span data-ttu-id="2c923-133">ID</span><span class="sxs-lookup"><span data-stu-id="2c923-133">id</span></span>|<span data-ttu-id="2c923-134">文字列</span><span class="sxs-lookup"><span data-stu-id="2c923-134">String</span></span>|<span data-ttu-id="2c923-135">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="2c923-135">The attachment ID.</span></span>|
|<span data-ttu-id="2c923-136">isInline</span><span class="sxs-lookup"><span data-stu-id="2c923-136">isInline</span></span>|<span data-ttu-id="2c923-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="2c923-137">Boolean</span></span>|<span data-ttu-id="2c923-138">インライン添付ファイルの場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="2c923-138">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="2c923-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c923-139">lastModifiedDateTime</span></span>|<span data-ttu-id="2c923-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c923-140">DateTimeOffset</span></span>|<span data-ttu-id="2c923-141">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="2c923-141">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="2c923-142">名前</span><span class="sxs-lookup"><span data-stu-id="2c923-142">name</span></span>|<span data-ttu-id="2c923-143">文字列</span><span class="sxs-lookup"><span data-stu-id="2c923-143">String</span></span>|<span data-ttu-id="2c923-144">埋め込み添付ファイルを表すアイコンの下に表示されるテキストを表す名前。これは、実際のファイル名にする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="2c923-144">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="2c923-145">サイズ</span><span class="sxs-lookup"><span data-stu-id="2c923-145">size</span></span>|<span data-ttu-id="2c923-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2c923-146">Int32</span></span>|<span data-ttu-id="2c923-147">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="2c923-147">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c923-148">関係</span><span class="sxs-lookup"><span data-stu-id="2c923-148">Relationships</span></span>
<span data-ttu-id="2c923-149">なし</span><span class="sxs-lookup"><span data-stu-id="2c923-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2c923-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c923-150">JSON representation</span></span>

<span data-ttu-id="2c923-151">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2c923-151">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
  "contentId": "string",
  "contentLocation": "string",
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
