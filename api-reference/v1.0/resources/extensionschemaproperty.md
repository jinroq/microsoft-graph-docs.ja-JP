# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="91687-101">extensionSchemaProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91687-101">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="91687-102">**extensionSchemaProperty** リソースを使用して、[schemaExtension](schemaextension.md) 定義の一部としてプロパティの名前とその種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="91687-102">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="91687-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91687-103">Properties</span></span>
| <span data-ttu-id="91687-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91687-104">Property</span></span>     | <span data-ttu-id="91687-105">型</span><span class="sxs-lookup"><span data-stu-id="91687-105">Type</span></span>   |<span data-ttu-id="91687-106">説明</span><span class="sxs-lookup"><span data-stu-id="91687-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91687-107">name</span><span class="sxs-lookup"><span data-stu-id="91687-107">name</span></span>|<span data-ttu-id="91687-108">String</span><span class="sxs-lookup"><span data-stu-id="91687-108">String</span></span>| <span data-ttu-id="91687-109">スキーマの拡張機能の一部として定義されている厳密に型指定されたプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="91687-109">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="91687-110">type</span><span class="sxs-lookup"><span data-stu-id="91687-110">type</span></span>|<span data-ttu-id="91687-111">String</span><span class="sxs-lookup"><span data-stu-id="91687-111">String</span></span>| <span data-ttu-id="91687-p101">スキーマの拡張機能の一部として定義されているプロパティの種類。使用可能な値は、*Binary、Boolean、DateTime、Integer**String* です。詳細については、次の表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91687-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="91687-115">サポート対象のプロパティ データ型</span><span class="sxs-lookup"><span data-stu-id="91687-115">Supported property data types</span></span> 
<span data-ttu-id="91687-116">スキーマ拡張機能でプロパティを定義する場合、次のデータ型がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="91687-116">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="91687-117">プロパティの種類</span><span class="sxs-lookup"><span data-stu-id="91687-117">Property Type</span></span> | <span data-ttu-id="91687-118">注釈</span><span class="sxs-lookup"><span data-stu-id="91687-118">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="91687-119">Binary</span><span class="sxs-lookup"><span data-stu-id="91687-119">Binary</span></span> | <span data-ttu-id="91687-120">最大 256 バイトです。</span><span class="sxs-lookup"><span data-stu-id="91687-120">256 bytes maximum.</span></span> |
| <span data-ttu-id="91687-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="91687-121">Boolean</span></span> | <span data-ttu-id="91687-122">連絡先、メッセージ、イベント、投稿ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91687-122">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="91687-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="91687-123">DateTime</span></span> | <span data-ttu-id="91687-p102">ISO 8601 形式で指定する必要があります。UTC で格納されます。</span><span class="sxs-lookup"><span data-stu-id="91687-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="91687-126">Integer</span><span class="sxs-lookup"><span data-stu-id="91687-126">Integer</span></span> | <span data-ttu-id="91687-127">32 ビット値です。</span><span class="sxs-lookup"><span data-stu-id="91687-127">A 32-bit integer value.</span></span> <span data-ttu-id="91687-128">連絡先、メッセージ、イベント、投稿ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91687-128">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="91687-129">String</span><span class="sxs-lookup"><span data-stu-id="91687-129">String</span></span> | <span data-ttu-id="91687-130">最大 256 文字です。</span><span class="sxs-lookup"><span data-stu-id="91687-130">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91687-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91687-131">JSON representation</span></span>
<span data-ttu-id="91687-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91687-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
