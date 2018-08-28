# <a name="imageinfo-resource-type"></a><span data-ttu-id="213d3-101">imageInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="213d3-101">imageInfo resource type</span></span>

<span data-ttu-id="213d3-102"> ** アクティビティ** オブジェクトの [visualInfo](../resources/projectrome_visualinfo.md) の一部の [ 属性](../resources/projectrome_activity.md) のプロパティを表すための複合型です。</span><span class="sxs-lookup"><span data-stu-id="213d3-102">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome_visualinfo.md) part of the [activity](../resources/projectrome_activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="213d3-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="213d3-103">Properties</span></span>

|<span data-ttu-id="213d3-104">名前</span><span class="sxs-lookup"><span data-stu-id="213d3-104">Name</span></span> | <span data-ttu-id="213d3-105">型</span><span class="sxs-lookup"><span data-stu-id="213d3-105">Type</span></span> | <span data-ttu-id="213d3-106">説明</span><span class="sxs-lookup"><span data-stu-id="213d3-106">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="213d3-107">iconUrl</span><span class="sxs-lookup"><span data-stu-id="213d3-107">iconurl</span></span> | <span data-ttu-id="213d3-108">文字列</span><span class="sxs-lookup"><span data-stu-id="213d3-108">String</span></span> | <span data-ttu-id="213d3-109">省略可能です。活動を生成するために使用するアプリケーションを表すアイコンをポイントする URI</span><span class="sxs-lookup"><span data-stu-id="213d3-109">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="213d3-110">alternateText</span><span class="sxs-lookup"><span data-stu-id="213d3-110">alternateText</span></span> | <span data-ttu-id="213d3-111">文字列</span><span class="sxs-lookup"><span data-stu-id="213d3-111">String</span></span> | <span data-ttu-id="213d3-112">省略可能です。イメージの alt テキストのアクセス可能なコンテンツ</span><span class="sxs-lookup"><span data-stu-id="213d3-112">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="213d3-113">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="213d3-113">addImageQuery</span></span> | <span data-ttu-id="213d3-114">ブーリアン</span><span class="sxs-lookup"><span data-stu-id="213d3-114">Boolean</span></span> | <span data-ttu-id="213d3-115">省略可能です。サーバーを指定するためのパラメーターは、パラメーターへの応答に動的にイメージをレンダリングすることです。</span><span class="sxs-lookup"><span data-stu-id="213d3-115">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="213d3-116">例: ハイコントラスト イメージ</span><span class="sxs-lookup"><span data-stu-id="213d3-116">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="213d3-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="213d3-117">JSON Representation</span></span>

<span data-ttu-id="213d3-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="213d3-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->