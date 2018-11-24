# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="8a0f9-101">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a0f9-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="8a0f9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a0f9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a0f9-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8a0f9-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8a0f9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a0f9-104">Properties</span></span>
|<span data-ttu-id="8a0f9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a0f9-105">Property</span></span>|<span data-ttu-id="8a0f9-106">型</span><span class="sxs-lookup"><span data-stu-id="8a0f9-106">Type</span></span>|<span data-ttu-id="8a0f9-107">説明</span><span class="sxs-lookup"><span data-stu-id="8a0f9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a0f9-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="8a0f9-108">movieRating</span></span>|[<span data-ttu-id="8a0f9-109">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="8a0f9-109">ratingUnitedKingdomMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdommoviestype.md)|<span data-ttu-id="8a0f9-110">評価の英国を選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="8a0f9-110">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="8a0f9-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="8a0f9-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="8a0f9-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="8a0f9-112">tvRating</span></span>|[<span data-ttu-id="8a0f9-113">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8a0f9-113">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="8a0f9-114">テレビの視聴制限が英国を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a0f9-114">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="8a0f9-115">可能な値は、`allAllowed`、`allBlocked`、`caution` です。</span><span class="sxs-lookup"><span data-stu-id="8a0f9-115">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a0f9-116">関係</span><span class="sxs-lookup"><span data-stu-id="8a0f9-116">Relationships</span></span>
<span data-ttu-id="8a0f9-117">なし</span><span class="sxs-lookup"><span data-stu-id="8a0f9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a0f9-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a0f9-118">JSON Representation</span></span>
<span data-ttu-id="8a0f9-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a0f9-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



