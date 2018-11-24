# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="54438-101">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54438-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="54438-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="54438-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54438-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="54438-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="54438-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54438-104">Properties</span></span>
|<span data-ttu-id="54438-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54438-105">Property</span></span>|<span data-ttu-id="54438-106">型</span><span class="sxs-lookup"><span data-stu-id="54438-106">Type</span></span>|<span data-ttu-id="54438-107">説明</span><span class="sxs-lookup"><span data-stu-id="54438-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54438-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="54438-108">movieRating</span></span>|[<span data-ttu-id="54438-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="54438-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="54438-110">評価のオーストラリアの選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="54438-110">Movies rating selected for Australia.</span></span> <span data-ttu-id="54438-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="54438-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="54438-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="54438-112">tvRating</span></span>|[<span data-ttu-id="54438-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="54438-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="54438-114">テレビの視聴制限がオーストラリアを選択します。</span><span class="sxs-lookup"><span data-stu-id="54438-114">TV rating selected for Australia.</span></span> <span data-ttu-id="54438-115">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="54438-115">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54438-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54438-116">Relationships</span></span>
<span data-ttu-id="54438-117">なし</span><span class="sxs-lookup"><span data-stu-id="54438-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="54438-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54438-118">JSON Representation</span></span>
<span data-ttu-id="54438-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54438-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



