# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="183b8-101">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="183b8-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="183b8-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="183b8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="183b8-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="183b8-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="183b8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="183b8-104">Properties</span></span>
|<span data-ttu-id="183b8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="183b8-105">Property</span></span>|<span data-ttu-id="183b8-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="183b8-106">Type</span></span>|<span data-ttu-id="183b8-107">説明</span><span class="sxs-lookup"><span data-stu-id="183b8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="183b8-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="183b8-108">movieRating</span></span>|[<span data-ttu-id="183b8-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="183b8-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="183b8-p101">オーストラリア向けに選ばれている映画のレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="183b8-p101">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="183b8-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="183b8-112">tvRating</span></span>|[<span data-ttu-id="183b8-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="183b8-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="183b8-p102">オーストラリア向けに選ばれているテレビのレーティング。可能な値:  `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="183b8-p102">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="183b8-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="183b8-116">Relationships</span></span>
<span data-ttu-id="183b8-117">なし</span><span class="sxs-lookup"><span data-stu-id="183b8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="183b8-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="183b8-118">JSON Representation</span></span>
<span data-ttu-id="183b8-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="183b8-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```








