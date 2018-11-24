# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="72d89-101">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="72d89-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="72d89-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="72d89-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72d89-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="72d89-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="72d89-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72d89-104">Properties</span></span>
|<span data-ttu-id="72d89-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72d89-105">Property</span></span>|<span data-ttu-id="72d89-106">型</span><span class="sxs-lookup"><span data-stu-id="72d89-106">Type</span></span>|<span data-ttu-id="72d89-107">説明</span><span class="sxs-lookup"><span data-stu-id="72d89-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72d89-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="72d89-108">movieRating</span></span>|[<span data-ttu-id="72d89-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="72d89-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="72d89-110">評価のニュージーランドを選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="72d89-110">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="72d89-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。</span><span class="sxs-lookup"><span data-stu-id="72d89-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="72d89-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="72d89-112">tvRating</span></span>|[<span data-ttu-id="72d89-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="72d89-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="72d89-114">テレビの視聴制限がニュージーランドを選択します。</span><span class="sxs-lookup"><span data-stu-id="72d89-114">TV rating selected for New Zealand.</span></span> <span data-ttu-id="72d89-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="72d89-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72d89-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="72d89-116">Relationships</span></span>
<span data-ttu-id="72d89-117">なし</span><span class="sxs-lookup"><span data-stu-id="72d89-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="72d89-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="72d89-118">JSON Representation</span></span>
<span data-ttu-id="72d89-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="72d89-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



