# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="cc10f-101">mediaContentRatingCanada リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc10f-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="cc10f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc10f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc10f-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cc10f-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cc10f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc10f-104">Properties</span></span>
|<span data-ttu-id="cc10f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc10f-105">Property</span></span>|<span data-ttu-id="cc10f-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="cc10f-106">Type</span></span>|<span data-ttu-id="cc10f-107">説明</span><span class="sxs-lookup"><span data-stu-id="cc10f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc10f-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="cc10f-108">movieRating</span></span>|[<span data-ttu-id="cc10f-109">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="cc10f-109">ratingCanadaMoviesType</span></span>](../resources/intune_deviceconfig_ratingcanadamoviestype.md)|<span data-ttu-id="cc10f-p101">カナダ向けに選択されている映画のレーティング。指定できある値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted` です。</span><span class="sxs-lookup"><span data-stu-id="cc10f-p101">Movies rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="cc10f-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="cc10f-112">tvRating</span></span>|[<span data-ttu-id="cc10f-113">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cc10f-113">ratingCanadaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingcanadatelevisiontype.md)|<span data-ttu-id="cc10f-p102">カナダ向けに選択されているテレビのレーティング。指定できる値は、`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18` です。</span><span class="sxs-lookup"><span data-stu-id="cc10f-p102">TV rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc10f-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc10f-116">Relationships</span></span>
<span data-ttu-id="cc10f-117">なし</span><span class="sxs-lookup"><span data-stu-id="cc10f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc10f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc10f-118">JSON Representation</span></span>
<span data-ttu-id="cc10f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc10f-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```








