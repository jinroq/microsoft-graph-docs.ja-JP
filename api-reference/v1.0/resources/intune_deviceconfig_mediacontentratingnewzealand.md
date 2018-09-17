# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="78502-101">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78502-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="78502-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="78502-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78502-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="78502-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="78502-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78502-104">Properties</span></span>
|<span data-ttu-id="78502-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78502-105">Property</span></span>|<span data-ttu-id="78502-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="78502-106">Type</span></span>|<span data-ttu-id="78502-107">説明</span><span class="sxs-lookup"><span data-stu-id="78502-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78502-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="78502-108">movieRating</span></span>|[<span data-ttu-id="78502-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="78502-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="78502-p101">評価のニュージーランドを選択したムービーです。使用可能な値: `allAllowed`、 `allBlocked`、 `general`、 `parentalGuidance`、 `mature`、 `agesAbove13`、 `agesAbove15`、 `agesAbove16`、 `agesAbove18`、 `restricted`、 `agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="78502-p101">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="78502-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="78502-112">tvRating</span></span>|[<span data-ttu-id="78502-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="78502-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="78502-p102">ニュージーランド向けに選択されているテレビのレーティング。可能な値: `allAllowed` 、`allBlocked` 、`general` 、`parentalGuidance` 、`adults` 。</span><span class="sxs-lookup"><span data-stu-id="78502-p102">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78502-116">関係</span><span class="sxs-lookup"><span data-stu-id="78502-116">Relationships</span></span>
<span data-ttu-id="78502-117">なし</span><span class="sxs-lookup"><span data-stu-id="78502-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78502-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78502-118">JSON Representation</span></span>
<span data-ttu-id="78502-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78502-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```








