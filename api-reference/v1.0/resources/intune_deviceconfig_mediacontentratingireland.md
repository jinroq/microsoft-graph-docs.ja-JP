# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="1f19c-101">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f19c-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="1f19c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f19c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f19c-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1f19c-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1f19c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f19c-104">Properties</span></span>
|<span data-ttu-id="1f19c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f19c-105">Property</span></span>|<span data-ttu-id="1f19c-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="1f19c-106">Type</span></span>|<span data-ttu-id="1f19c-107">説明</span><span class="sxs-lookup"><span data-stu-id="1f19c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f19c-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="1f19c-108">movieRating</span></span>|[<span data-ttu-id="1f19c-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="1f19c-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="1f19c-110">アイルランド向けに選択された映画の視聴制限です。</span><span class="sxs-lookup"><span data-stu-id="1f19c-110">Movies rating selected for Ireland Possible values are: , , , , , , , .</span></span> <span data-ttu-id="1f19c-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="1f19c-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`, , , , or .</span></span>|
|<span data-ttu-id="1f19c-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="1f19c-112">tvRating</span></span>|[<span data-ttu-id="1f19c-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1f19c-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="1f19c-114">アイルランド向けに選択されたテレビの視聴制限です。</span><span class="sxs-lookup"><span data-stu-id="1f19c-114">TV rating selected for Ireland Possible values are: , , , , , , .</span></span> <span data-ttu-id="1f19c-115">指定できる値は、`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature` です。</span><span class="sxs-lookup"><span data-stu-id="1f19c-115">The possible values are `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`, , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f19c-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f19c-116">Relationships</span></span>
<span data-ttu-id="1f19c-117">なし</span><span class="sxs-lookup"><span data-stu-id="1f19c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f19c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f19c-118">JSON Representation</span></span>
<span data-ttu-id="1f19c-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f19c-119">Here is a JSON representation of the resource.</span></span>
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



