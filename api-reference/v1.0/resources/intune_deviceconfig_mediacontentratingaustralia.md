# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="2a223-101">mediaContentRatingAustralia リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a223-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="2a223-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a223-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a223-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2a223-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2a223-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a223-104">Properties</span></span>
|<span data-ttu-id="2a223-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a223-105">Property</span></span>|<span data-ttu-id="2a223-106">型</span><span class="sxs-lookup"><span data-stu-id="2a223-106">Type</span></span>|<span data-ttu-id="2a223-107">説明</span><span class="sxs-lookup"><span data-stu-id="2a223-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a223-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="2a223-108">movieRating</span></span>|<span data-ttu-id="2a223-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2a223-109">String</span></span>|<span data-ttu-id="2a223-110">オーストラリア向けに選択されている映画のレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="2a223-110">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="2a223-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="2a223-111">tvRating</span></span>|<span data-ttu-id="2a223-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2a223-112">String</span></span>|<span data-ttu-id="2a223-113">オーストラリア向けに選択されているテレビのレーティング。可能な値: `allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="2a223-113">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a223-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a223-114">Relationships</span></span>
<span data-ttu-id="2a223-115">なし</span><span class="sxs-lookup"><span data-stu-id="2a223-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a223-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a223-116">JSON Representation</span></span>
<span data-ttu-id="2a223-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a223-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



