# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="59003-101">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59003-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="59003-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59003-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59003-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="59003-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="59003-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59003-104">Properties</span></span>
|<span data-ttu-id="59003-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59003-105">Property</span></span>|<span data-ttu-id="59003-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="59003-106">Type</span></span>|<span data-ttu-id="59003-107">説明</span><span class="sxs-lookup"><span data-stu-id="59003-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59003-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="59003-108">movieRating</span></span>|[<span data-ttu-id="59003-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="59003-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="59003-p101">日本向けに選択されている映画のレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="59003-p101">Movies rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="59003-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="59003-112">tvRating</span></span>|[<span data-ttu-id="59003-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="59003-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="59003-p102">日本向けに選択されているテレビのレーティング。可能な値: `allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="59003-p102">TV rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59003-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59003-116">Relationships</span></span>
<span data-ttu-id="59003-117">なし</span><span class="sxs-lookup"><span data-stu-id="59003-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59003-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59003-118">JSON Representation</span></span>
<span data-ttu-id="59003-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59003-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```








