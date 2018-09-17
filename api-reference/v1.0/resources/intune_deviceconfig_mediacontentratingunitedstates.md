# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="dd115-101">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dd115-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="dd115-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd115-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd115-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dd115-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="dd115-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd115-104">Properties</span></span>
|<span data-ttu-id="dd115-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd115-105">Property</span></span>|<span data-ttu-id="dd115-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="dd115-106">Type</span></span>|<span data-ttu-id="dd115-107">説明</span><span class="sxs-lookup"><span data-stu-id="dd115-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd115-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="dd115-108">movieRating</span></span>|[<span data-ttu-id="dd115-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="dd115-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="dd115-p101">評価の米国の選択したムービーです。使用可能な値: `allAllowed`、 `allBlocked`、 `general`、 `parentalGuidance`、 `parentalGuidance13`、 `restricted`、 `adults`。</span><span class="sxs-lookup"><span data-stu-id="dd115-p101">Movies rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="dd115-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="dd115-112">tvRating</span></span>|[<span data-ttu-id="dd115-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="dd115-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="dd115-p102">テレビの視聴制限はアメリカ合衆国を選択します。使用可能な値: `allAllowed`、 `allBlocked`、 `childrenAll`、 `childrenAbove7`、 `general`、 `parentalGuidance`、 `childrenAbove14`、 `adults`。</span><span class="sxs-lookup"><span data-stu-id="dd115-p102">TV rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd115-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dd115-116">Relationships</span></span>
<span data-ttu-id="dd115-117">なし</span><span class="sxs-lookup"><span data-stu-id="dd115-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dd115-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd115-118">JSON Representation</span></span>
<span data-ttu-id="dd115-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dd115-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```








