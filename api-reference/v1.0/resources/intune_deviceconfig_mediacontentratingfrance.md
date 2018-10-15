# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="cc961-101">mediaContentRatingFrance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc961-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="cc961-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc961-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc961-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cc961-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cc961-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc961-104">Properties</span></span>
|<span data-ttu-id="cc961-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc961-105">Property</span></span>|<span data-ttu-id="cc961-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="cc961-106">Type</span></span>|<span data-ttu-id="cc961-107">説明</span><span class="sxs-lookup"><span data-stu-id="cc961-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc961-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="cc961-108">movieRating</span></span>|[<span data-ttu-id="cc961-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="cc961-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="cc961-p101">フランス向けに選ばれている映画のレーティング。指定できる値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="cc961-p101">Movies rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="cc961-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="cc961-112">tvRating</span></span>|[<span data-ttu-id="cc961-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cc961-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="cc961-p102">フランス向けに選ばれているテレビのレーティング。指定できる値: `allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="cc961-p102">TV rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc961-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc961-116">Relationships</span></span>
<span data-ttu-id="cc961-117">なし</span><span class="sxs-lookup"><span data-stu-id="cc961-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc961-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc961-118">JSON Representation</span></span>
<span data-ttu-id="cc961-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc961-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```








