# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="8756b-101">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8756b-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="8756b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8756b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8756b-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8756b-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8756b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8756b-104">Properties</span></span>
|<span data-ttu-id="8756b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8756b-105">Property</span></span>|<span data-ttu-id="8756b-106">型</span><span class="sxs-lookup"><span data-stu-id="8756b-106">Type</span></span>|<span data-ttu-id="8756b-107">説明</span><span class="sxs-lookup"><span data-stu-id="8756b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8756b-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="8756b-108">movieRating</span></span>|[<span data-ttu-id="8756b-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="8756b-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="8756b-110">評価のアイルランドの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="8756b-110">Movies rating selected for Ireland.</span></span> <span data-ttu-id="8756b-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="8756b-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="8756b-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="8756b-112">tvRating</span></span>|[<span data-ttu-id="8756b-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8756b-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="8756b-114">テレビの視聴制限はアイルランドのために選択します。</span><span class="sxs-lookup"><span data-stu-id="8756b-114">TV rating selected for Ireland.</span></span> <span data-ttu-id="8756b-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="8756b-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8756b-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8756b-116">Relationships</span></span>
<span data-ttu-id="8756b-117">なし</span><span class="sxs-lookup"><span data-stu-id="8756b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8756b-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8756b-118">JSON Representation</span></span>
<span data-ttu-id="8756b-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8756b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



