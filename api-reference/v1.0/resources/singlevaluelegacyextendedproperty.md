# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="d7c6d-101">singleValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7c6d-101">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="d7c6d-102">単一値が含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="d7c6d-102">An extended property that contains a single value.</span></span> 

<span data-ttu-id="d7c6d-103">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7c6d-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="d7c6d-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7c6d-104">Methods</span></span>

| <span data-ttu-id="d7c6d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7c6d-105">Method</span></span>           | <span data-ttu-id="d7c6d-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d7c6d-106">Return Type</span></span>    |<span data-ttu-id="d7c6d-107">説明</span><span class="sxs-lookup"><span data-stu-id="d7c6d-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7c6d-108">投稿</span><span class="sxs-lookup"><span data-stu-id="d7c6d-108">Post</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) | <span data-ttu-id="d7c6d-109">サポートされているリソース インスタンス: [メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、または [contactFolder](../resources/contactfolder.md) (ただし、グループ[投稿](../resources/post.md)を除く)。</span><span class="sxs-lookup"><span data-stu-id="d7c6d-109">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="d7c6d-110">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **singleValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="d7c6d-110">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="d7c6d-111">取得</span><span class="sxs-lookup"><span data-stu-id="d7c6d-111">Get</span></span>](../api/singlevaluelegacyextendedproperty_get.md) |<span data-ttu-id="d7c6d-112">サポートされているリソースのインスタンス ([メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、[contactFolder](../resources/contactfolder.md)、またはグループ[投稿](../resources/post.md)) のいずれか、またはそれらのコレクション、あるいは [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) オブジェクトで拡張されているインスタンスなどのいずれか。</span><span class="sxs-lookup"><span data-stu-id="d7c6d-112">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="d7c6d-113">または `$filter` を使用して拡張プロパティでリソース インスタンスを取得します。`$expand`</span><span class="sxs-lookup"><span data-stu-id="d7c6d-113">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7c6d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7c6d-114">Properties</span></span>
| <span data-ttu-id="d7c6d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7c6d-115">Property</span></span>     | <span data-ttu-id="d7c6d-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="d7c6d-116">Type</span></span>   |<span data-ttu-id="d7c6d-117">説明</span><span class="sxs-lookup"><span data-stu-id="d7c6d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7c6d-118">ID</span><span class="sxs-lookup"><span data-stu-id="d7c6d-118">id</span></span>|<span data-ttu-id="d7c6d-119">文字列</span><span class="sxs-lookup"><span data-stu-id="d7c6d-119">string</span></span>|<span data-ttu-id="d7c6d-p101">プロパティの識別に使用されるプロパティ ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d7c6d-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="d7c6d-122">値</span><span class="sxs-lookup"><span data-stu-id="d7c6d-122">value</span></span>|<span data-ttu-id="d7c6d-123">文字列</span><span class="sxs-lookup"><span data-stu-id="d7c6d-123">string</span></span>|<span data-ttu-id="d7c6d-124">プロパティ値。</span><span class="sxs-lookup"><span data-stu-id="d7c6d-124">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7c6d-125">関係</span><span class="sxs-lookup"><span data-stu-id="d7c6d-125">Relationships</span></span>
<span data-ttu-id="d7c6d-126">なし</span><span class="sxs-lookup"><span data-stu-id="d7c6d-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d7c6d-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7c6d-127">JSON representation</span></span>

<span data-ttu-id="d7c6d-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d7c6d-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->