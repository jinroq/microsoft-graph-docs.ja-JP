# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="024f0-101">mediaContentRatingIreland リソースの種類</span><span class="sxs-lookup"><span data-stu-id="024f0-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="024f0-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="024f0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="024f0-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="024f0-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="024f0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="024f0-104">Properties</span></span>
|<span data-ttu-id="024f0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="024f0-105">Property</span></span>|<span data-ttu-id="024f0-106">型</span><span class="sxs-lookup"><span data-stu-id="024f0-106">Type</span></span>|<span data-ttu-id="024f0-107">説明</span><span class="sxs-lookup"><span data-stu-id="024f0-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="024f0-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="024f0-108">movieRating</span></span>|<span data-ttu-id="024f0-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="024f0-109">String</span></span>|<span data-ttu-id="024f0-110">アイルランド向けに選択されている映画のレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="024f0-110">Movies rating selected for Ireland Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="024f0-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="024f0-111">tvRating</span></span>|<span data-ttu-id="024f0-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="024f0-112">String</span></span>|<span data-ttu-id="024f0-113">アイルランド向けに選択されているテレビのレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="024f0-113">TV rating selected for Ireland Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="024f0-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="024f0-114">Relationships</span></span>
<span data-ttu-id="024f0-115">なし</span><span class="sxs-lookup"><span data-stu-id="024f0-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="024f0-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="024f0-116">JSON Representation</span></span>
<span data-ttu-id="024f0-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="024f0-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



