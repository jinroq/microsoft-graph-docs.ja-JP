# <a name="referenceattachment-resource-type"></a><span data-ttu-id="c1686-101">referenceAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1686-101">referenceAttachment resource type</span></span>

<span data-ttu-id="c1686-102">OneDrive for Business のクラウド ドライブまたは他のサポートされている保存場所にあり、イベント、メッセージ、または投稿にアタッチされているファイル (テキスト ファイルまたは Word 文書など) へのリンク。</span><span class="sxs-lookup"><span data-stu-id="c1686-102">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="c1686-103">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="c1686-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c1686-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1686-104">Methods</span></span>

| <span data-ttu-id="c1686-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1686-105">Method</span></span>       | <span data-ttu-id="c1686-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c1686-106">Return Type</span></span>  |<span data-ttu-id="c1686-107">説明</span><span class="sxs-lookup"><span data-stu-id="c1686-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1686-108">取得</span><span class="sxs-lookup"><span data-stu-id="c1686-108">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="c1686-109">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="c1686-109">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="c1686-110">referenceAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c1686-110">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="c1686-111">削除</span><span class="sxs-lookup"><span data-stu-id="c1686-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="c1686-112">なし</span><span class="sxs-lookup"><span data-stu-id="c1686-112">None</span></span> |<span data-ttu-id="c1686-113">referenceAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="c1686-113">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c1686-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1686-114">Properties</span></span>
| <span data-ttu-id="c1686-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1686-115">Property</span></span>     | <span data-ttu-id="c1686-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="c1686-116">Type</span></span>   |<span data-ttu-id="c1686-117">説明</span><span class="sxs-lookup"><span data-stu-id="c1686-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1686-118">contentType</span><span class="sxs-lookup"><span data-stu-id="c1686-118">contentType</span></span>|<span data-ttu-id="c1686-119">文字列</span><span class="sxs-lookup"><span data-stu-id="c1686-119">String</span></span>|<span data-ttu-id="c1686-120">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="c1686-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="c1686-121">id</span><span class="sxs-lookup"><span data-stu-id="c1686-121">id</span></span>|<span data-ttu-id="c1686-122">文字列</span><span class="sxs-lookup"><span data-stu-id="c1686-122">String</span></span>|<span data-ttu-id="c1686-p101">添付ファイル ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c1686-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="c1686-125">isInline</span><span class="sxs-lookup"><span data-stu-id="c1686-125">isInline</span></span>|<span data-ttu-id="c1686-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="c1686-126">Boolean</span></span>|<span data-ttu-id="c1686-127">添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="c1686-127">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="c1686-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1686-128">lastModifiedDateTime</span></span>|<span data-ttu-id="c1686-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1686-129">DateTimeOffset</span></span>|<span data-ttu-id="c1686-p102">添付ファイルが最後に変更された日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c1686-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c1686-133">name</span><span class="sxs-lookup"><span data-stu-id="c1686-133">name</span></span>|<span data-ttu-id="c1686-134">文字列</span><span class="sxs-lookup"><span data-stu-id="c1686-134">String</span></span>|<span data-ttu-id="c1686-p103">埋め込まれた添付ファイルを表すアイコンの下に表示されるテキスト。実際のファイル名である必要はありません。</span><span class="sxs-lookup"><span data-stu-id="c1686-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="c1686-137">size</span><span class="sxs-lookup"><span data-stu-id="c1686-137">size</span></span>|<span data-ttu-id="c1686-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c1686-138">Int32</span></span>|<span data-ttu-id="c1686-139">添付ファイルのメッセージに格納されているメタデータのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="c1686-139">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="c1686-140">この値は実際のファイルのサイズを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="c1686-140">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1686-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1686-141">Relationships</span></span>
<span data-ttu-id="c1686-142">なし</span><span class="sxs-lookup"><span data-stu-id="c1686-142">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="c1686-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1686-143">JSON representation</span></span>

<span data-ttu-id="c1686-144">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c1686-144">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.referenceAttachment"
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
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
