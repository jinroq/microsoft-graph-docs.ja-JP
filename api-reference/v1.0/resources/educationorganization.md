# <a name="educationorganization-resource-type"></a><span data-ttu-id="8b183-101">教育組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b183-101">educationOrganization resource type</span></span>

<span data-ttu-id="8b183-102">教育セクター内の異なる種類の組織の共通性をモデル化するために使用する抽象エンティティです。</span><span class="sxs-lookup"><span data-stu-id="8b183-102">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="8b183-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b183-103">Properties</span></span>
| <span data-ttu-id="8b183-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b183-104">Property</span></span>     | <span data-ttu-id="8b183-105">型</span><span class="sxs-lookup"><span data-stu-id="8b183-105">Type</span></span>   |<span data-ttu-id="8b183-106">説明</span><span class="sxs-lookup"><span data-stu-id="8b183-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b183-107">description</span><span class="sxs-lookup"><span data-stu-id="8b183-107">description</span></span>|<span data-ttu-id="8b183-108">文字列</span><span class="sxs-lookup"><span data-stu-id="8b183-108">String</span></span>| <span data-ttu-id="8b183-109">組織の説明</span><span class="sxs-lookup"><span data-stu-id="8b183-109">Organization description.</span></span>|
|<span data-ttu-id="8b183-110">displayName</span><span class="sxs-lookup"><span data-stu-id="8b183-110">displayName</span></span>|<span data-ttu-id="8b183-111">文字列</span><span class="sxs-lookup"><span data-stu-id="8b183-111">String</span></span>| <span data-ttu-id="8b183-112">組織の表示名</span><span class="sxs-lookup"><span data-stu-id="8b183-112">Organization display name.</span></span>|
|<span data-ttu-id="8b183-113">externalSource</span><span class="sxs-lookup"><span data-stu-id="8b183-113">externalSource</span></span>|<span data-ttu-id="8b183-114">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="8b183-114">educationExternalSource</span></span>| <span data-ttu-id="8b183-115">この組織を作成したソース。</span><span class="sxs-lookup"><span data-stu-id="8b183-115">Source where this organization was created from.</span></span> <span data-ttu-id="8b183-116">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8b183-116">The possible values are `sis`, `manual`, or `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b183-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8b183-117">Relationships</span></span>
<span data-ttu-id="8b183-118">なし。</span><span class="sxs-lookup"><span data-stu-id="8b183-118">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8b183-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b183-119">JSON representation</span></span>

<span data-ttu-id="8b183-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b183-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->