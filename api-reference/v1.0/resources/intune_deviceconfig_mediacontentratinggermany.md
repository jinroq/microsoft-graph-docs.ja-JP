# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="6b421-101">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b421-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="6b421-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b421-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b421-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6b421-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6b421-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b421-104">Properties</span></span>
|<span data-ttu-id="6b421-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b421-105">Property</span></span>|<span data-ttu-id="6b421-106">型</span><span class="sxs-lookup"><span data-stu-id="6b421-106">Type</span></span>|<span data-ttu-id="6b421-107">説明</span><span class="sxs-lookup"><span data-stu-id="6b421-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b421-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="6b421-108">movieRating</span></span>|[<span data-ttu-id="6b421-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="6b421-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="6b421-110">映画がドイツの選択を評価します。</span><span class="sxs-lookup"><span data-stu-id="6b421-110">Movies rating selected for Germany.</span></span> <span data-ttu-id="6b421-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="6b421-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="6b421-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="6b421-112">tvRating</span></span>|[<span data-ttu-id="6b421-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6b421-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="6b421-114">テレビの視聴制限がドイツを選択します。</span><span class="sxs-lookup"><span data-stu-id="6b421-114">TV rating selected for Germany.</span></span> <span data-ttu-id="6b421-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="6b421-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b421-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6b421-116">Relationships</span></span>
<span data-ttu-id="6b421-117">なし</span><span class="sxs-lookup"><span data-stu-id="6b421-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b421-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b421-118">JSON Representation</span></span>
<span data-ttu-id="6b421-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6b421-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



