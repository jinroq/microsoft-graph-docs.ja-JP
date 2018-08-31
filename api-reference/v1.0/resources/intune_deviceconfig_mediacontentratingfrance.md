# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="646c9-101">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="646c9-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="646c9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="646c9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="646c9-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="646c9-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="646c9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="646c9-104">Properties</span></span>
|<span data-ttu-id="646c9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="646c9-105">Property</span></span>|<span data-ttu-id="646c9-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="646c9-106">Type</span></span>|<span data-ttu-id="646c9-107">説明</span><span class="sxs-lookup"><span data-stu-id="646c9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="646c9-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="646c9-108">movieRating</span></span>|[<span data-ttu-id="646c9-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="646c9-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="646c9-110">フランスの映画レイティング</span><span class="sxs-lookup"><span data-stu-id="646c9-110">Movies rating selected for France Possible values are: , , , , , .</span></span> <span data-ttu-id="646c9-111">指定できる値は、`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="646c9-111">The possible values are `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`, , , , , , or .</span></span>|
|<span data-ttu-id="646c9-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="646c9-112">tvRating</span></span>|[<span data-ttu-id="646c9-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="646c9-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="646c9-114">フランスのテレビ番組のレイティング</span><span class="sxs-lookup"><span data-stu-id="646c9-114">TV rating selected for France Possible values are: , , , , , .</span></span> <span data-ttu-id="646c9-115">指定できる値は、`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="646c9-115">The possible values are `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="646c9-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="646c9-116">Relationships</span></span>
<span data-ttu-id="646c9-117">なし</span><span class="sxs-lookup"><span data-stu-id="646c9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="646c9-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="646c9-118">JSON Representation</span></span>
<span data-ttu-id="646c9-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="646c9-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



