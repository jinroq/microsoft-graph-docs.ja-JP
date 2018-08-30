# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="2ee4e-101">inferenceClassification リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ee4e-101">inferenceClassification resource type</span></span>

<span data-ttu-id="2ee4e-102">ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。</span><span class="sxs-lookup"><span data-stu-id="2ee4e-102">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="2ee4e-103">詳しくは、「[優先受信トレイを管理する](manage_focused_inbox.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ee4e-103">For more information, see [Manage Focused Inbox](manage_focused_inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="2ee4e-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ee4e-104">Methods</span></span>

| <span data-ttu-id="2ee4e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ee4e-105">Method</span></span>           | <span data-ttu-id="2ee4e-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2ee4e-106">Return Type</span></span>    |<span data-ttu-id="2ee4e-107">説明</span><span class="sxs-lookup"><span data-stu-id="2ee4e-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ee4e-108">inferenceClassificationOverride を作成する</span><span class="sxs-lookup"><span data-stu-id="2ee4e-108">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification_post_overrides.md) |[<span data-ttu-id="2ee4e-109">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="2ee4e-109">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="2ee4e-p101">SMTP アドレスで示される送信者のオーバーライドを作成します。この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。</span><span class="sxs-lookup"><span data-stu-id="2ee4e-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="2ee4e-112">オーバーライドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2ee4e-112">List overrides</span></span>](../api/inferenceclassification_list_overrides.md) |<span data-ttu-id="2ee4e-113">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ee4e-113">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="2ee4e-114">ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。</span><span class="sxs-lookup"><span data-stu-id="2ee4e-114">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ee4e-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ee4e-115">Properties</span></span>
| <span data-ttu-id="2ee4e-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ee4e-116">Property</span></span>     | <span data-ttu-id="2ee4e-117">タイプ</span><span class="sxs-lookup"><span data-stu-id="2ee4e-117">Type</span></span>   |<span data-ttu-id="2ee4e-118">説明</span><span class="sxs-lookup"><span data-stu-id="2ee4e-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ee4e-119">ID</span><span class="sxs-lookup"><span data-stu-id="2ee4e-119">id</span></span>|<span data-ttu-id="2ee4e-120">文字列</span><span class="sxs-lookup"><span data-stu-id="2ee4e-120">string</span></span>| <span data-ttu-id="2ee4e-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2ee4e-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ee4e-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ee4e-122">Relationships</span></span>
| <span data-ttu-id="2ee4e-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ee4e-123">Relationship</span></span> | <span data-ttu-id="2ee4e-124">型</span><span class="sxs-lookup"><span data-stu-id="2ee4e-124">Type</span></span>   |<span data-ttu-id="2ee4e-125">説明</span><span class="sxs-lookup"><span data-stu-id="2ee4e-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ee4e-126">overrides</span><span class="sxs-lookup"><span data-stu-id="2ee4e-126">overrides</span></span>|<span data-ttu-id="2ee4e-127">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ee4e-127">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="2ee4e-p102">ユーザーが、`focused` または `other` の特定の方法で特定の差出人からのメッセージを常時分類するための一連のオーバーライド。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2ee4e-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ee4e-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ee4e-131">JSON representation</span></span>

<span data-ttu-id="2ee4e-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ee4e-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->