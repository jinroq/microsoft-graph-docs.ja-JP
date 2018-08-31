# <a name="visualinfo-resource-type"></a><span data-ttu-id="ea7ad-101">visualInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ea7ad-101">visualInfo resource type</span></span>

<span data-ttu-id="ea7ad-102"> [activity](../resources/projectrome_activity.md) オブジェクトの **visualElements** プロパティを表すための複合型です。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-102">A complex type for representing the **attribution** property in the [visualInfo part of the activity](../resources/projectrome_activity.md) object.</span></span>

<span data-ttu-id="ea7ad-103">各ユーザーのアクティビティは、アダプティブ カードとしてタイムラインに表示されます。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-103">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="ea7ad-104">アプリ開発者は、アプリ内で行われたアクティビティの概要をキャプチャするカスタム カードを提供するよう奨励されています。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-104">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="ea7ad-105">これは、コンテンツ プロパティでカスタム JSON カードを提供することにより可能です。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-105">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="ea7ad-106">アダプティブ カードを含むビジュアル メタデータに加えて、アプリは、将来的な再エンゲージメントにつながる新たなアクティビティを提供する目的でユーザーのアクティビティに関する推論を構築するのに使用できるコンテンツ メタデータを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-106">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="ea7ad-107">これは、コンテンツを記述するのに schema.org プロパティを利用する JSON オブジェクトを提供する目的で、アクティビティの contentInfo プロパティを使用することにより可能です。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-107">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="ea7ad-108">カスタム カードが提供されていない場合は、displayText および description プロパティを使って単純なカードが生成されます。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-108">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="ea7ad-109">アプリ内で最高のコンテンツをショーケースするためにカスタム カードが推奨されています。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-109">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="ea7ad-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea7ad-110">Properties</span></span>

|<span data-ttu-id="ea7ad-111">名前</span><span class="sxs-lookup"><span data-stu-id="ea7ad-111">Name</span></span> | <span data-ttu-id="ea7ad-112">型</span><span class="sxs-lookup"><span data-stu-id="ea7ad-112">Type</span></span> | <span data-ttu-id="ea7ad-113">説明</span><span class="sxs-lookup"><span data-stu-id="ea7ad-113">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="ea7ad-114">displayText</span><span class="sxs-lookup"><span data-stu-id="ea7ad-114">displayText</span></span> | <span data-ttu-id="ea7ad-115">文字列</span><span class="sxs-lookup"><span data-stu-id="ea7ad-115">String</span></span> | <span data-ttu-id="ea7ad-116">必須。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-116">Required.</span></span> <span data-ttu-id="ea7ad-117">ユーザーの一意のアクティビティの簡潔な説明文 (アクティビティがドキュメントの作成を参照する場合は、文書名など)</span><span class="sxs-lookup"><span data-stu-id="ea7ad-117">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="ea7ad-118">description</span><span class="sxs-lookup"><span data-stu-id="ea7ad-118">description</span></span> | <span data-ttu-id="ea7ad-119">文字列</span><span class="sxs-lookup"><span data-stu-id="ea7ad-119">String</span></span> | <span data-ttu-id="ea7ad-120">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-120">Optional.</span></span> <span data-ttu-id="ea7ad-121">ユーザーのユニーク アクティビティのより長い説明文 (ドキュメント名、最初の文、および / またはメタデータなど)</span><span class="sxs-lookup"><span data-stu-id="ea7ad-121">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="ea7ad-122">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="ea7ad-122">background-color</span></span> | <span data-ttu-id="ea7ad-123">文字列</span><span class="sxs-lookup"><span data-stu-id="ea7ad-123">String</span></span> | <span data-ttu-id="ea7ad-124">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-124">Optional.</span></span> <span data-ttu-id="ea7ad-125">UI でアクティビティを示すために使用される背景色で、アクティビティのアプリケーション ソースのブランド色です。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-125">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="ea7ad-126">有効な 16 進数の色でなければなりません</span><span class="sxs-lookup"><span data-stu-id="ea7ad-126">Must be a valid hex color</span></span>|
|<span data-ttu-id="ea7ad-127">content</span><span class="sxs-lookup"><span data-stu-id="ea7ad-127">content</span></span> | <span data-ttu-id="ea7ad-128">型指定されていない JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="ea7ad-128">Untyped JSON object</span></span> | <span data-ttu-id="ea7ad-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-129">Optional.</span></span> <span data-ttu-id="ea7ad-130">カスタム データ - Windows シェル UI のアクティビティを表示するためのカスタム コンテンツを提供するのに使用される JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="ea7ad-130">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="ea7ad-131">attribution</span><span class="sxs-lookup"><span data-stu-id="ea7ad-131">attribution</span></span> | <span data-ttu-id="ea7ad-132">[imageInfo](../resources/projectrome_imageinfo.md)</span><span class="sxs-lookup"><span data-stu-id="ea7ad-132">Added [imageInfo](../resources/projectrome_imageinfo.md)</span></span> | <span data-ttu-id="ea7ad-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-133">Optional.</span></span> <span data-ttu-id="ea7ad-134">アクティビティを生成するのに使用されるアプリケーションを表すアイコンを示すのに使用される JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="ea7ad-134">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea7ad-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ea7ad-135">JSON Representation</span></span>

<span data-ttu-id="ea7ad-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ea7ad-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
