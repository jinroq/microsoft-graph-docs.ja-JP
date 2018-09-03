# <a name="outlookitem-resource-type"></a><span data-ttu-id="17b30-101">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17b30-101">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="17b30-102">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17b30-102">JSON representation</span></span>

<span data-ttu-id="17b30-103">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="17b30-103">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="17b30-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17b30-104">Properties</span></span>
| <span data-ttu-id="17b30-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17b30-105">Property</span></span>     | <span data-ttu-id="17b30-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="17b30-106">Type</span></span>   |<span data-ttu-id="17b30-107">説明</span><span class="sxs-lookup"><span data-stu-id="17b30-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17b30-108">categories</span><span class="sxs-lookup"><span data-stu-id="17b30-108">categories</span></span>|<span data-ttu-id="17b30-109">String コレクション</span><span class="sxs-lookup"><span data-stu-id="17b30-109">String collection</span></span>|<span data-ttu-id="17b30-110">項目に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="17b30-110">The categories associated with the message.</span></span>|
|<span data-ttu-id="17b30-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="17b30-111">changeKey</span></span>|<span data-ttu-id="17b30-112">String</span><span class="sxs-lookup"><span data-stu-id="17b30-112">String</span></span>|<span data-ttu-id="17b30-113">項目のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="17b30-113">Gets the version number of the item version.</span></span> <span data-ttu-id="17b30-114">項目が変更されるたびに、changeKey も同様に変更します。</span><span class="sxs-lookup"><span data-stu-id="17b30-114">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="17b30-115">これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="17b30-115">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="17b30-116">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="17b30-116">Read-only.</span></span>|
|<span data-ttu-id="17b30-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17b30-117">createdDateTime</span></span>|<span data-ttu-id="17b30-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17b30-118">DateTimeOffset</span></span>|<span data-ttu-id="17b30-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="17b30-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="17b30-121">id</span><span class="sxs-lookup"><span data-stu-id="17b30-121">id</span></span>|<span data-ttu-id="17b30-122">文字列</span><span class="sxs-lookup"><span data-stu-id="17b30-122">String</span></span>| <span data-ttu-id="17b30-123">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="17b30-123">Read-only.</span></span>|
|<span data-ttu-id="17b30-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17b30-124">lastModifiedDateTime</span></span>|<span data-ttu-id="17b30-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17b30-125">DateTimeOffset</span></span>|<span data-ttu-id="17b30-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="17b30-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="17b30-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17b30-128">Relationships</span></span>
<span data-ttu-id="17b30-129">なし</span><span class="sxs-lookup"><span data-stu-id="17b30-129">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
