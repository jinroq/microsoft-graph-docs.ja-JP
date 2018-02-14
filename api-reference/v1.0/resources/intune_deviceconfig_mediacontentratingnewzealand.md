# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="3c0ea-101">mediaContentRatingNewZealand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c0ea-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="3c0ea-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c0ea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c0ea-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c0ea-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3c0ea-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c0ea-104">Properties</span></span>
|<span data-ttu-id="3c0ea-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c0ea-105">Property</span></span>|<span data-ttu-id="3c0ea-106">型</span><span class="sxs-lookup"><span data-stu-id="3c0ea-106">Type</span></span>|<span data-ttu-id="3c0ea-107">説明</span><span class="sxs-lookup"><span data-stu-id="3c0ea-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c0ea-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="3c0ea-108">movieRating</span></span>|<span data-ttu-id="3c0ea-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3c0ea-109">String</span></span>|<span data-ttu-id="3c0ea-110">ニュージーランド向けに選択されている映画のレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="3c0ea-110">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="3c0ea-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="3c0ea-111">tvRating</span></span>|<span data-ttu-id="3c0ea-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3c0ea-112">String</span></span>|<span data-ttu-id="3c0ea-113">ニュージーランド向けに選択されているテレビのレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="3c0ea-113">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c0ea-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3c0ea-114">Relationships</span></span>
<span data-ttu-id="3c0ea-115">なし</span><span class="sxs-lookup"><span data-stu-id="3c0ea-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c0ea-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c0ea-116">JSON Representation</span></span>
<span data-ttu-id="3c0ea-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3c0ea-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



