# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="d8830-101">mediaContentRatingGermany リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8830-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="d8830-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8830-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8830-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d8830-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d8830-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8830-104">Properties</span></span>
|<span data-ttu-id="d8830-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8830-105">Property</span></span>|<span data-ttu-id="d8830-106">型</span><span class="sxs-lookup"><span data-stu-id="d8830-106">Type</span></span>|<span data-ttu-id="d8830-107">説明</span><span class="sxs-lookup"><span data-stu-id="d8830-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8830-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="d8830-108">movieRating</span></span>|<span data-ttu-id="d8830-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d8830-109">String</span></span>|<span data-ttu-id="d8830-110">ドイツ向けに選択されている映画のレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="d8830-110">Movies rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="d8830-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="d8830-111">tvRating</span></span>|<span data-ttu-id="d8830-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d8830-112">String</span></span>|<span data-ttu-id="d8830-113">ドイツ向けに選択されているテレビのレーティング。可能な値: `allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="d8830-113">TV rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8830-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8830-114">Relationships</span></span>
<span data-ttu-id="d8830-115">なし</span><span class="sxs-lookup"><span data-stu-id="d8830-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d8830-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8830-116">JSON Representation</span></span>
<span data-ttu-id="d8830-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8830-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



