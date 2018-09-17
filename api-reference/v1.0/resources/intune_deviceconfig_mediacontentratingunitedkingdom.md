# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="21efe-101">mediaContentRatingUnitedKingdom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21efe-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="21efe-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="21efe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21efe-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="21efe-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="21efe-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21efe-104">Properties</span></span>
|<span data-ttu-id="21efe-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21efe-105">Property</span></span>|<span data-ttu-id="21efe-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="21efe-106">Type</span></span>|<span data-ttu-id="21efe-107">説明</span><span class="sxs-lookup"><span data-stu-id="21efe-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21efe-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="21efe-108">movieRating</span></span>|[<span data-ttu-id="21efe-109">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="21efe-109">ratingUnitedKingdomMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdommoviestype.md)|<span data-ttu-id="21efe-p101">イギリス向けに選択されている映画のレーティング。使用可能な値: `allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="21efe-p101">Movies rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="21efe-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="21efe-112">tvRating</span></span>|[<span data-ttu-id="21efe-113">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="21efe-113">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="21efe-p102">イギリス向けに選択されているテレビのレーティング。使用可能な値: `allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="21efe-p102">TV rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21efe-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21efe-116">Relationships</span></span>
<span data-ttu-id="21efe-117">なし</span><span class="sxs-lookup"><span data-stu-id="21efe-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21efe-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21efe-118">JSON Representation</span></span>
<span data-ttu-id="21efe-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21efe-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```








