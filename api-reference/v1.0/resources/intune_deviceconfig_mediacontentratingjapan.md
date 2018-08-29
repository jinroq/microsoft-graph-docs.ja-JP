# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="45c80-101">mediaContentRatingJapan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45c80-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="45c80-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="45c80-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45c80-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="45c80-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="45c80-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45c80-104">Properties</span></span>
|<span data-ttu-id="45c80-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45c80-105">Property</span></span>|<span data-ttu-id="45c80-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="45c80-106">Type</span></span>|<span data-ttu-id="45c80-107">説明</span><span class="sxs-lookup"><span data-stu-id="45c80-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45c80-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="45c80-108">movieRating</span></span>|[<span data-ttu-id="45c80-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="45c80-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="45c80-110">日本向けに選択されている映画のレーティング。</span><span class="sxs-lookup"><span data-stu-id="45c80-110">Movies rating selected for Japan Possible values are: , , , , , .</span></span> <span data-ttu-id="45c80-111">指定できる値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="45c80-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`, , , , , , or .</span></span>|
|<span data-ttu-id="45c80-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="45c80-112">tvRating</span></span>|[<span data-ttu-id="45c80-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="45c80-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="45c80-114">日本向けに選択されているテレビのレーティング。</span><span class="sxs-lookup"><span data-stu-id="45c80-114">TV rating selected for Japan Possible values are: , , .</span></span> <span data-ttu-id="45c80-115">指定できる値: `allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="45c80-115">The possible values are `allAllowed`, `allBlocked`, or `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45c80-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="45c80-116">Relationships</span></span>
<span data-ttu-id="45c80-117">なし</span><span class="sxs-lookup"><span data-stu-id="45c80-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="45c80-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45c80-118">JSON Representation</span></span>
<span data-ttu-id="45c80-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="45c80-119">Here is a JSON representation of the resource.</span></span>
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



