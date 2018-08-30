# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="9f37b-101">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f37b-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="9f37b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f37b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f37b-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f37b-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="9f37b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f37b-104">Properties</span></span>
|<span data-ttu-id="9f37b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f37b-105">Property</span></span>|<span data-ttu-id="9f37b-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="9f37b-106">Type</span></span>|<span data-ttu-id="9f37b-107">説明</span><span class="sxs-lookup"><span data-stu-id="9f37b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f37b-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="9f37b-108">movieRating</span></span>|[<span data-ttu-id="9f37b-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="9f37b-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="9f37b-110">オーストラリア向けに選択された映画規制</span><span class="sxs-lookup"><span data-stu-id="9f37b-110">Movies rating selected for Australia Possible values are: , , , , , , .</span></span> <span data-ttu-id="9f37b-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="9f37b-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`, , , , , or .</span></span>|
|<span data-ttu-id="9f37b-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="9f37b-112">tvRating</span></span>|[<span data-ttu-id="9f37b-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9f37b-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="9f37b-114">オーストラリア向けに選択されたテレビ規制</span><span class="sxs-lookup"><span data-stu-id="9f37b-114">TV rating selected for Australia Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="9f37b-115">可能な値は、`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence` です。</span><span class="sxs-lookup"><span data-stu-id="9f37b-115">The possible values are `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`, , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f37b-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f37b-116">Relationships</span></span>
<span data-ttu-id="9f37b-117">なし</span><span class="sxs-lookup"><span data-stu-id="9f37b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f37b-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f37b-118">JSON Representation</span></span>
<span data-ttu-id="9f37b-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f37b-119">Here is a JSON representation of the resource.</span></span>
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



