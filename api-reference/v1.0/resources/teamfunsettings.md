# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="9a3f6-101">teamFunSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a3f6-101">teamFunSettings resource type</span></span>



<span data-ttu-id="9a3f6-102">Giphy、memes、および[チーム](team.md)のステッカーを構成する設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a3f6-102">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9a3f6-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a3f6-103">Properties</span></span>
| <span data-ttu-id="9a3f6-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a3f6-104">Property</span></span>     | <span data-ttu-id="9a3f6-105">型</span><span class="sxs-lookup"><span data-stu-id="9a3f6-105">Type</span></span>   |<span data-ttu-id="9a3f6-106">説明</span><span class="sxs-lookup"><span data-stu-id="9a3f6-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a3f6-107">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="9a3f6-107">allowGiphy</span></span>|<span data-ttu-id="9a3f6-108">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a3f6-108">Boolean</span></span>|<span data-ttu-id="9a3f6-109">場合 true の場合、有効にする Giphy の使用を設定します。</span><span class="sxs-lookup"><span data-stu-id="9a3f6-109">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="9a3f6-110">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="9a3f6-110">giphyContentRating</span></span>|<span data-ttu-id="9a3f6-111">文字列 (列挙型)</span><span class="sxs-lookup"><span data-stu-id="9a3f6-111">String (enum)</span></span>|<span data-ttu-id="9a3f6-112">コンテンツの規制を Giphy。</span><span class="sxs-lookup"><span data-stu-id="9a3f6-112">Giphy content rating.</span></span> <span data-ttu-id="9a3f6-113">使用可能な値は、`moderate`、`strict` です。</span><span class="sxs-lookup"><span data-stu-id="9a3f6-113">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="9a3f6-114">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="9a3f6-114">allowStickersAndMemes</span></span>|<span data-ttu-id="9a3f6-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a3f6-115">Boolean</span></span>|<span data-ttu-id="9a3f6-116">場合は true、ステッカー、memes など、ユーザーに設定します。</span><span class="sxs-lookup"><span data-stu-id="9a3f6-116">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="9a3f6-117">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="9a3f6-117">allowCustomMemes</span></span>|<span data-ttu-id="9a3f6-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a3f6-118">Boolean</span></span>|<span data-ttu-id="9a3f6-119">場合に true を設定する、カスタムの memes を含むようにユーザーをできるようにする設定です。</span><span class="sxs-lookup"><span data-stu-id="9a3f6-119">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a3f6-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a3f6-120">JSON representation</span></span>

<span data-ttu-id="9a3f6-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a3f6-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
