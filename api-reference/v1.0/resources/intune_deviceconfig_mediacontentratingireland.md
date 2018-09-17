# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="3476f-101">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3476f-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="3476f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3476f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3476f-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3476f-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3476f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3476f-104">Properties</span></span>
|<span data-ttu-id="3476f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3476f-105">Property</span></span>|<span data-ttu-id="3476f-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="3476f-106">Type</span></span>|<span data-ttu-id="3476f-107">説明</span><span class="sxs-lookup"><span data-stu-id="3476f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3476f-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="3476f-108">movieRating</span></span>|[<span data-ttu-id="3476f-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="3476f-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="3476f-p101">アイルランド向けに選択されているテレビのレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="3476f-p101">Movies rating selected for Ireland Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="3476f-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="3476f-112">tvRating</span></span>|[<span data-ttu-id="3476f-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3476f-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="3476f-p102">アイルランド向けに選択されているテレビのレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="3476f-p102">TV rating selected for Ireland Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3476f-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3476f-116">Relationships</span></span>
<span data-ttu-id="3476f-117">なし</span><span class="sxs-lookup"><span data-stu-id="3476f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3476f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3476f-118">JSON Representation</span></span>
<span data-ttu-id="3476f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3476f-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```








