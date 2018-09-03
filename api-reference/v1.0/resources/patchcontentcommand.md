# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="414a2-101">patchContentCommand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="414a2-101">patchContentCommand resource type</span></span>

<span data-ttu-id="414a2-102">PATCH 要求で OneNote ページに加える変更。</span><span class="sxs-lookup"><span data-stu-id="414a2-102">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="414a2-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="414a2-103">JSON representation</span></span>

<span data-ttu-id="414a2-104">以下は、リソースの JSON 表記です。[PATCH pages/{id}\`](../api/page_update.md) 要求の本文に送信されます。</span><span class="sxs-lookup"><span data-stu-id="414a2-104">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page_update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="414a2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="414a2-105">Properties</span></span>
| <span data-ttu-id="414a2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="414a2-106">Property</span></span>     | <span data-ttu-id="414a2-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="414a2-107">Type</span></span>   |<span data-ttu-id="414a2-108">説明</span><span class="sxs-lookup"><span data-stu-id="414a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="414a2-109">操作</span><span class="sxs-lookup"><span data-stu-id="414a2-109">action</span></span>|<span data-ttu-id="414a2-110">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="414a2-110">onenotePatchActionType values</span></span>|<span data-ttu-id="414a2-111">ターゲット要素で実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="414a2-111">The action to perform on the target element.</span></span> <span data-ttu-id="414a2-112">使用可能な値は、`replace`、`append`、`delete`、`insert`、`prepend` です。</span><span class="sxs-lookup"><span data-stu-id="414a2-112">The possible values are `replace`, `append`, `delete`, `insert`, , , , , , , , or `prepend`.</span></span>|
|<span data-ttu-id="414a2-113">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="414a2-113">content</span></span>|<span data-ttu-id="414a2-114">文字列</span><span class="sxs-lookup"><span data-stu-id="414a2-114">String</span></span>|<span data-ttu-id="414a2-p102">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="414a2-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="414a2-117">位置</span><span class="sxs-lookup"><span data-stu-id="414a2-117">position</span></span>|<span data-ttu-id="414a2-118">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="414a2-118">onenotePatchInsertPosition values</span></span>|<span data-ttu-id="414a2-119">指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。</span><span class="sxs-lookup"><span data-stu-id="414a2-119">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="414a2-120">使用可能な値は、`after` (既定値) または `before` です。</span><span class="sxs-lookup"><span data-stu-id="414a2-120">The possible values are , , , , , , , , , , , or .</span></span>|
|<span data-ttu-id="414a2-121">ターゲット</span><span class="sxs-lookup"><span data-stu-id="414a2-121">target</span></span>|<span data-ttu-id="414a2-122">文字列</span><span class="sxs-lookup"><span data-stu-id="414a2-122">String</span></span>|<span data-ttu-id="414a2-p104">更新する要素。要素の `#<data-id>` または生成された `<id>`、または `body` か `title` のキーワードでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="414a2-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
