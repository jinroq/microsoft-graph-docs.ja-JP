# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="16dcb-101">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="16dcb-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="16dcb-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16dcb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16dcb-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="16dcb-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="16dcb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16dcb-104">Properties</span></span>
|<span data-ttu-id="16dcb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16dcb-105">Property</span></span>|<span data-ttu-id="16dcb-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="16dcb-106">Type</span></span>|<span data-ttu-id="16dcb-107">説明</span><span class="sxs-lookup"><span data-stu-id="16dcb-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16dcb-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="16dcb-108">movieRating</span></span>|[<span data-ttu-id="16dcb-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="16dcb-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="16dcb-110">ドイツ向けに選択された映画規制</span><span class="sxs-lookup"><span data-stu-id="16dcb-110">Movies rating selected for Germany Possible values are: , , , , , , .</span></span> <span data-ttu-id="16dcb-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="16dcb-111">The possible values are `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`, , , , , or .</span></span>|
|<span data-ttu-id="16dcb-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="16dcb-112">tvRating</span></span>|[<span data-ttu-id="16dcb-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="16dcb-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="16dcb-114">ドイツ向けに選択されたテレビ規制</span><span class="sxs-lookup"><span data-stu-id="16dcb-114">TV rating selected for Germany Possible values are: , , , , , , .</span></span> <span data-ttu-id="16dcb-115">可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="16dcb-115">The possible values are `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`, , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="16dcb-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="16dcb-116">Relationships</span></span>
<span data-ttu-id="16dcb-117">なし</span><span class="sxs-lookup"><span data-stu-id="16dcb-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="16dcb-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16dcb-118">JSON Representation</span></span>
<span data-ttu-id="16dcb-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="16dcb-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



