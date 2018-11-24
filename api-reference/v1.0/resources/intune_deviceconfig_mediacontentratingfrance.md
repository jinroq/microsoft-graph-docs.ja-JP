# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="3ae2a-101">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3ae2a-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="3ae2a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ae2a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ae2a-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3ae2a-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3ae2a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ae2a-104">Properties</span></span>
|<span data-ttu-id="3ae2a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ae2a-105">Property</span></span>|<span data-ttu-id="3ae2a-106">型</span><span class="sxs-lookup"><span data-stu-id="3ae2a-106">Type</span></span>|<span data-ttu-id="3ae2a-107">説明</span><span class="sxs-lookup"><span data-stu-id="3ae2a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ae2a-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="3ae2a-108">movieRating</span></span>|[<span data-ttu-id="3ae2a-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="3ae2a-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="3ae2a-110">映画はフランスの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="3ae2a-110">Movies rating selected for France.</span></span> <span data-ttu-id="3ae2a-111">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="3ae2a-111">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="3ae2a-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="3ae2a-112">tvRating</span></span>|[<span data-ttu-id="3ae2a-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3ae2a-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="3ae2a-114">テレビの視聴制限がフランス用に選択します。</span><span class="sxs-lookup"><span data-stu-id="3ae2a-114">TV rating selected for France.</span></span> <span data-ttu-id="3ae2a-115">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="3ae2a-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ae2a-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ae2a-116">Relationships</span></span>
<span data-ttu-id="3ae2a-117">なし</span><span class="sxs-lookup"><span data-stu-id="3ae2a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3ae2a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ae2a-118">JSON Representation</span></span>
<span data-ttu-id="3ae2a-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ae2a-119">Here is a JSON representation of the resource.</span></span>
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



