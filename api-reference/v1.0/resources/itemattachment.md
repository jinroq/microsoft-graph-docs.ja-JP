# <a name="itemattachment-resource-type"></a><span data-ttu-id="d8fac-101">itemAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8fac-101">itemAttachment resource type</span></span>

<span data-ttu-id="d8fac-102">連絡先、イベント、または別のイベントに添付されたメッセージ、メッセージ、または投稿です。</span><span class="sxs-lookup"><span data-stu-id="d8fac-102">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="d8fac-103">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="d8fac-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d8fac-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8fac-104">Methods</span></span>

| <span data-ttu-id="d8fac-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8fac-105">Method</span></span>       | <span data-ttu-id="d8fac-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8fac-106">Return Type</span></span>  |<span data-ttu-id="d8fac-107">説明</span><span class="sxs-lookup"><span data-stu-id="d8fac-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8fac-108">取得</span><span class="sxs-lookup"><span data-stu-id="d8fac-108">Get</span></span>](../api/attachment_get.md) | <span data-ttu-id="d8fac-109">[ItemAttachment](itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="d8fac-109">[itemAttachment](itemattachment.md),</span></span> |<span data-ttu-id="d8fac-110">itemAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d8fac-110">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="d8fac-111">削除</span><span class="sxs-lookup"><span data-stu-id="d8fac-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="d8fac-112">なし</span><span class="sxs-lookup"><span data-stu-id="d8fac-112">None</span></span> |<span data-ttu-id="d8fac-113">itemAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d8fac-113">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d8fac-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8fac-114">Properties</span></span>
| <span data-ttu-id="d8fac-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8fac-115">Property</span></span>     | <span data-ttu-id="d8fac-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="d8fac-116">Type</span></span>   |<span data-ttu-id="d8fac-117">説明</span><span class="sxs-lookup"><span data-stu-id="d8fac-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8fac-118">contentType</span><span class="sxs-lookup"><span data-stu-id="d8fac-118">contentType</span></span>|<span data-ttu-id="d8fac-119">文字列</span><span class="sxs-lookup"><span data-stu-id="d8fac-119">String</span></span>|<span data-ttu-id="d8fac-120">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="d8fac-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="d8fac-121">id</span><span class="sxs-lookup"><span data-stu-id="d8fac-121">id</span></span>|<span data-ttu-id="d8fac-122">文字列</span><span class="sxs-lookup"><span data-stu-id="d8fac-122">String</span></span>| <span data-ttu-id="d8fac-123">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="d8fac-123">The attachment ID.</span></span>|
|<span data-ttu-id="d8fac-124">isInline</span><span class="sxs-lookup"><span data-stu-id="d8fac-124">isInline</span></span>|<span data-ttu-id="d8fac-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="d8fac-125">Boolean</span></span>|<span data-ttu-id="d8fac-126">添付ファイルがインライン (アイテムの本文に埋め込まれた画像など) の場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="d8fac-126">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="d8fac-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8fac-127">lastModifiedDateTime</span></span>|<span data-ttu-id="d8fac-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8fac-128">DateTimeOffset</span></span>|<span data-ttu-id="d8fac-129">添付ファイルが変更された最後の日時です。</span><span class="sxs-lookup"><span data-stu-id="d8fac-129">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="d8fac-130">name</span><span class="sxs-lookup"><span data-stu-id="d8fac-130">name</span></span>|<span data-ttu-id="d8fac-131">文字列</span><span class="sxs-lookup"><span data-stu-id="d8fac-131">String</span></span>|<span data-ttu-id="d8fac-132">添付ファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="d8fac-132">The display name of the attachment.</span></span>|
|<span data-ttu-id="d8fac-133">size</span><span class="sxs-lookup"><span data-stu-id="d8fac-133">size</span></span>|<span data-ttu-id="d8fac-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fac-134">Int32</span></span>|<span data-ttu-id="d8fac-135">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="d8fac-135">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8fac-136">関係</span><span class="sxs-lookup"><span data-stu-id="d8fac-136">Relationships</span></span>
| <span data-ttu-id="d8fac-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8fac-137">Relationship</span></span> | <span data-ttu-id="d8fac-138">型</span><span class="sxs-lookup"><span data-stu-id="d8fac-138">Type</span></span>   |<span data-ttu-id="d8fac-139">説明</span><span class="sxs-lookup"><span data-stu-id="d8fac-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8fac-140">item</span><span class="sxs-lookup"><span data-stu-id="d8fac-140">item</span></span>|[<span data-ttu-id="d8fac-141">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="d8fac-141">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="d8fac-p101">添付されたメッセージまたはイベントです。ナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="d8fac-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8fac-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8fac-144">JSON representation</span></span>

<span data-ttu-id="d8fac-145">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d8fac-145">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
