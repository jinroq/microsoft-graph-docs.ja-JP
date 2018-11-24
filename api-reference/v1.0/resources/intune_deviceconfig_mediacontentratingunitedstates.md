# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="f38f9-101">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f38f9-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="f38f9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f38f9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f38f9-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f38f9-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f38f9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f38f9-104">Properties</span></span>
|<span data-ttu-id="f38f9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f38f9-105">Property</span></span>|<span data-ttu-id="f38f9-106">型</span><span class="sxs-lookup"><span data-stu-id="f38f9-106">Type</span></span>|<span data-ttu-id="f38f9-107">説明</span><span class="sxs-lookup"><span data-stu-id="f38f9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f38f9-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="f38f9-108">movieRating</span></span>|[<span data-ttu-id="f38f9-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="f38f9-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="f38f9-110">評価の米国の選択したムービーです。</span><span class="sxs-lookup"><span data-stu-id="f38f9-110">Movies rating selected for United States.</span></span> <span data-ttu-id="f38f9-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="f38f9-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="f38f9-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="f38f9-112">tvRating</span></span>|[<span data-ttu-id="f38f9-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f38f9-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="f38f9-114">テレビの視聴制限はアメリカ合衆国を選択します。</span><span class="sxs-lookup"><span data-stu-id="f38f9-114">TV rating selected for United States.</span></span> <span data-ttu-id="f38f9-115">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="f38f9-115">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f38f9-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f38f9-116">Relationships</span></span>
<span data-ttu-id="f38f9-117">なし</span><span class="sxs-lookup"><span data-stu-id="f38f9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f38f9-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f38f9-118">JSON Representation</span></span>
<span data-ttu-id="f38f9-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f38f9-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



