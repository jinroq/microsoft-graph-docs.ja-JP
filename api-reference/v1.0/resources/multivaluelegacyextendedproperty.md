# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="a2691-101">multiValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2691-101">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="a2691-102">値のコレクションが含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="a2691-102">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="a2691-103">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2691-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="a2691-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2691-104">Methods</span></span>

| <span data-ttu-id="a2691-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2691-105">Method</span></span>           | <span data-ttu-id="a2691-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a2691-106">Return Type</span></span>    |<span data-ttu-id="a2691-107">説明</span><span class="sxs-lookup"><span data-stu-id="a2691-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2691-108">投稿</span><span class="sxs-lookup"><span data-stu-id="a2691-108">Post</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | <span data-ttu-id="a2691-p101">サポートされているリソース インスタンス: [メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、または [contactFolder](../resources/contactfolder.md)。グループ[投稿](../resources/post.md) はサポートされていませんので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="a2691-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="a2691-111">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **multiValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="a2691-111">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="a2691-112">取得</span><span class="sxs-lookup"><span data-stu-id="a2691-112">Get</span></span>](../api/multivaluelegacyextendedproperty_get.md) |<span data-ttu-id="a2691-113">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) オブジェクトで拡張されたサポートされているリソースのインスタンス ([メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、[contactFolder](../resources/contactfolder.md)、またはグループ[投稿](../resources/post.md))。</span><span class="sxs-lookup"><span data-stu-id="a2691-113">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="a2691-114">`$expand` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2691-114">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2691-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2691-115">Properties</span></span>
| <span data-ttu-id="a2691-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2691-116">Property</span></span>     | <span data-ttu-id="a2691-117">タイプ</span><span class="sxs-lookup"><span data-stu-id="a2691-117">Type</span></span>   |<span data-ttu-id="a2691-118">説明</span><span class="sxs-lookup"><span data-stu-id="a2691-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2691-119">ID</span><span class="sxs-lookup"><span data-stu-id="a2691-119">id</span></span>|<span data-ttu-id="a2691-120">文字列</span><span class="sxs-lookup"><span data-stu-id="a2691-120">string</span></span>|<span data-ttu-id="a2691-p102">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2691-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="a2691-123">値</span><span class="sxs-lookup"><span data-stu-id="a2691-123">value</span></span>|<span data-ttu-id="a2691-124">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a2691-124">string collection</span></span>|<span data-ttu-id="a2691-125">プロパティ値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a2691-125">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2691-126">関係</span><span class="sxs-lookup"><span data-stu-id="a2691-126">Relationships</span></span>
<span data-ttu-id="a2691-127">なし</span><span class="sxs-lookup"><span data-stu-id="a2691-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a2691-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2691-128">JSON representation</span></span>

<span data-ttu-id="a2691-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2691-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->