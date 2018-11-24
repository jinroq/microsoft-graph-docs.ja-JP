# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="14518-101">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14518-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="14518-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="14518-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14518-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="14518-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="14518-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14518-104">Properties</span></span>
|<span data-ttu-id="14518-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14518-105">Property</span></span>|<span data-ttu-id="14518-106">型</span><span class="sxs-lookup"><span data-stu-id="14518-106">Type</span></span>|<span data-ttu-id="14518-107">説明</span><span class="sxs-lookup"><span data-stu-id="14518-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14518-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="14518-108">movieRating</span></span>|[<span data-ttu-id="14518-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="14518-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="14518-110">評価日本の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="14518-110">Movies rating selected for Japan.</span></span> <span data-ttu-id="14518-111">使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="14518-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="14518-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="14518-112">tvRating</span></span>|[<span data-ttu-id="14518-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="14518-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="14518-114">テレビの視聴制限が日本用に選択します。</span><span class="sxs-lookup"><span data-stu-id="14518-114">TV rating selected for Japan.</span></span> <span data-ttu-id="14518-115">可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。</span><span class="sxs-lookup"><span data-stu-id="14518-115">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14518-116">関係</span><span class="sxs-lookup"><span data-stu-id="14518-116">Relationships</span></span>
<span data-ttu-id="14518-117">なし</span><span class="sxs-lookup"><span data-stu-id="14518-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14518-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14518-118">JSON Representation</span></span>
<span data-ttu-id="14518-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14518-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



