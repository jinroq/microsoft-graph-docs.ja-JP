# <a name="itembody-resource-type"></a><span data-ttu-id="87ec8-101">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="87ec8-101">itemBody resource type</span></span>

<span data-ttu-id="87ec8-102">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="87ec8-102">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="87ec8-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87ec8-103">Properties</span></span>
| <span data-ttu-id="87ec8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87ec8-104">Property</span></span>     | <span data-ttu-id="87ec8-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="87ec8-105">Type</span></span>   |<span data-ttu-id="87ec8-106">説明</span><span class="sxs-lookup"><span data-stu-id="87ec8-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87ec8-107">content</span><span class="sxs-lookup"><span data-stu-id="87ec8-107">content</span></span>|<span data-ttu-id="87ec8-108">文字列</span><span class="sxs-lookup"><span data-stu-id="87ec8-108">String</span></span>|<span data-ttu-id="87ec8-109">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="87ec8-109">The content of the item.</span></span>|
|<span data-ttu-id="87ec8-110">contentType</span><span class="sxs-lookup"><span data-stu-id="87ec8-110">contentType</span></span>|<span data-ttu-id="87ec8-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="87ec8-111">BodyType</span></span>|<span data-ttu-id="87ec8-p101">コンテンツの種類。可能な値は、`Text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="87ec8-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87ec8-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="87ec8-114">JSON representation</span></span>

<span data-ttu-id="87ec8-115">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="87ec8-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
