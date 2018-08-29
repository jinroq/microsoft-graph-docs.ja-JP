# <a name="attachment-resource-type"></a><span data-ttu-id="32865-101">添付ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32865-101">attachment resource type</span></span>

<span data-ttu-id="32865-102">関連コンテンツを添付ファイルの形式で[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、または[投稿](../resources/post.md)に追加できます。</span><span class="sxs-lookup"><span data-stu-id="32865-102">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="32865-103">**attachment** は、次の派生型の添付ファイルの基本リソースです。</span><span class="sxs-lookup"><span data-stu-id="32865-103">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="32865-104">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)</span><span class="sxs-lookup"><span data-stu-id="32865-104">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="32865-105">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)</span><span class="sxs-lookup"><span data-stu-id="32865-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="32865-106">ファイルへのリンク ([referenceAttachment](../resources/referenceAttachment.md) リソース)</span><span class="sxs-lookup"><span data-stu-id="32865-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="32865-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="32865-107">Methods</span></span>

<span data-ttu-id="32865-108">次のメソッドは、派生型の添付ファイル (**fileAttachment**、**itemAttachment**、または **referenceAttachment**) のすべてに適用されます。</span><span class="sxs-lookup"><span data-stu-id="32865-108">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="32865-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="32865-109">Method</span></span>       | <span data-ttu-id="32865-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="32865-110">Return Type</span></span>  |<span data-ttu-id="32865-111">説明</span><span class="sxs-lookup"><span data-stu-id="32865-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32865-112">添付ファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="32865-112">Get attachment</span></span>](../api/attachment_get.md) | [<span data-ttu-id="32865-113">attachment</span><span class="sxs-lookup"><span data-stu-id="32865-113">attachment</span></span>](attachment.md) |<span data-ttu-id="32865-114">イベント、メッセージ、または投稿に添付されている添付ファイルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="32865-114">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="32865-115">イベントに添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="32865-115">Add attachment to an event</span></span>](../api/event_post_attachments.md) | [<span data-ttu-id="32865-116">attachment</span><span class="sxs-lookup"><span data-stu-id="32865-116">attachment</span></span>](attachment.md) |<span data-ttu-id="32865-117">ファイル、アイテム、またはリンクの添付ファイルをイベントに追加します。</span><span class="sxs-lookup"><span data-stu-id="32865-117">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="32865-118">メッセージに添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="32865-118">Add attachment to a message</span></span>](../api/message_post_attachments.md) | [<span data-ttu-id="32865-119">attachment</span><span class="sxs-lookup"><span data-stu-id="32865-119">attachment</span></span>](attachment.md) |<span data-ttu-id="32865-120">ファイル、アイテム、またはリンクの添付ファイルをメッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="32865-120">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="32865-121">投稿に添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="32865-121">Add attachment to a post</span></span>](../api/post_post_attachments.md) | [<span data-ttu-id="32865-122">attachment</span><span class="sxs-lookup"><span data-stu-id="32865-122">attachment</span></span>](attachment.md) |<span data-ttu-id="32865-123">ファイル、アイテム、またはリンクの添付ファイルを投稿に追加します。</span><span class="sxs-lookup"><span data-stu-id="32865-123">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="32865-124">イベントの添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="32865-124">List attachments of an event</span></span>](../api/event_list_attachments.md) | <span data-ttu-id="32865-125">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="32865-125">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="32865-126">イベントの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="32865-126">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="32865-127">メッセージの添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="32865-127">List attachments of a message</span></span>](../api/message_list_attachments.md) | <span data-ttu-id="32865-128">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="32865-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="32865-129">メッセージの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="32865-129">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="32865-130">投稿の添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="32865-130">List attachments of a post</span></span>](../api/post_list_attachments.md) | <span data-ttu-id="32865-131">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="32865-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="32865-132">投稿の添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="32865-132">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="32865-133">削除</span><span class="sxs-lookup"><span data-stu-id="32865-133">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="32865-134">なし</span><span class="sxs-lookup"><span data-stu-id="32865-134">None</span></span> |<span data-ttu-id="32865-135">イベント、メッセージ、または投稿の添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="32865-135">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="32865-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32865-136">Properties</span></span>

<span data-ttu-id="32865-p101">次に、添付ファイル リソースの基本プロパティを示します。他のプロパティについては、特定の種類の添付ファイル ([fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md)、または [referenceAttachment](../resources/referenceAttachment.md)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32865-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceAttachment.md)) for additional properties.</span></span>

| <span data-ttu-id="32865-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32865-139">Property</span></span>     | <span data-ttu-id="32865-140">タイプ</span><span class="sxs-lookup"><span data-stu-id="32865-140">Type</span></span>   |<span data-ttu-id="32865-141">説明</span><span class="sxs-lookup"><span data-stu-id="32865-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32865-142">contentType</span><span class="sxs-lookup"><span data-stu-id="32865-142">contentType</span></span>|<span data-ttu-id="32865-143">文字列</span><span class="sxs-lookup"><span data-stu-id="32865-143">String</span></span>|<span data-ttu-id="32865-144">MIME タイプ。</span><span class="sxs-lookup"><span data-stu-id="32865-144">The MIME type.</span></span>|
|<span data-ttu-id="32865-145">ID</span><span class="sxs-lookup"><span data-stu-id="32865-145">id</span></span>|<span data-ttu-id="32865-146">文字列</span><span class="sxs-lookup"><span data-stu-id="32865-146">String</span></span>| <span data-ttu-id="32865-147">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="32865-147">Read-only.</span></span>|
|<span data-ttu-id="32865-148">isInline</span><span class="sxs-lookup"><span data-stu-id="32865-148">isInline</span></span>|<span data-ttu-id="32865-149">ブール値</span><span class="sxs-lookup"><span data-stu-id="32865-149">Boolean</span></span>|<span data-ttu-id="32865-150">`true` 添付ファイルがインライン添付ファイルの場合は `true`、それ以外の場合は `false`。</span><span class="sxs-lookup"><span data-stu-id="32865-150">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="32865-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32865-151">lastModifiedDateTime</span></span>|<span data-ttu-id="32865-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32865-152">DateTimeOffset</span></span>|<span data-ttu-id="32865-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="32865-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="32865-155">name</span><span class="sxs-lookup"><span data-stu-id="32865-155">name</span></span>|<span data-ttu-id="32865-156">文字列</span><span class="sxs-lookup"><span data-stu-id="32865-156">String</span></span>|<span data-ttu-id="32865-157">添付ファイルのファイル名。</span><span class="sxs-lookup"><span data-stu-id="32865-157">The attachment's file name.</span></span>|
|<span data-ttu-id="32865-158">size</span><span class="sxs-lookup"><span data-stu-id="32865-158">size</span></span>|<span data-ttu-id="32865-159">Int32</span><span class="sxs-lookup"><span data-stu-id="32865-159">Int32</span></span>|<span data-ttu-id="32865-160">添付ファイルの長さ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="32865-160">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32865-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32865-161">Relationships</span></span>
<span data-ttu-id="32865-162">なし</span><span class="sxs-lookup"><span data-stu-id="32865-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32865-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32865-163">JSON representation</span></span>

<span data-ttu-id="32865-164">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="32865-164">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
}-->

```json
{
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
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
