# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="b8a04-101">mediaContentRatingUnitedStates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8a04-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="b8a04-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8a04-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8a04-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b8a04-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b8a04-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8a04-104">Properties</span></span>
|<span data-ttu-id="b8a04-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8a04-105">Property</span></span>|<span data-ttu-id="b8a04-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="b8a04-106">Type</span></span>|<span data-ttu-id="b8a04-107">説明</span><span class="sxs-lookup"><span data-stu-id="b8a04-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8a04-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="b8a04-108">movieRating</span></span>|[<span data-ttu-id="b8a04-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="b8a04-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="b8a04-110">米国向けに選択された映画規制。</span><span class="sxs-lookup"><span data-stu-id="b8a04-110">Movies rating selected for United States Possible values are: , , , , , , .</span></span> <span data-ttu-id="b8a04-111">可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="b8a04-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`, , , , , or .</span></span>|
|<span data-ttu-id="b8a04-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="b8a04-112">tvRating</span></span>|[<span data-ttu-id="b8a04-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b8a04-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="b8a04-114">米国向けに選択されたテレビ規制。</span><span class="sxs-lookup"><span data-stu-id="b8a04-114">TV rating selected for United States Possible values are: , , , , , , , .</span></span> <span data-ttu-id="b8a04-115">可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。</span><span class="sxs-lookup"><span data-stu-id="b8a04-115">The possible values are `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`, , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8a04-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8a04-116">Relationships</span></span>
<span data-ttu-id="b8a04-117">なし</span><span class="sxs-lookup"><span data-stu-id="b8a04-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8a04-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8a04-118">JSON Representation</span></span>
<span data-ttu-id="b8a04-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8a04-119">Here is a JSON representation of the resource.</span></span>
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



