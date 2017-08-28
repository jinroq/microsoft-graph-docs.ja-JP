# <a name="assignedlicense-resource-type"></a><span data-ttu-id="4b43f-101">assignedLicense リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b43f-101">assignedLicense resource type</span></span>

<span data-ttu-id="4b43f-p101">ユーザーに割り当てられているライセンスを表します。[ユーザー](user.md) エンティティの **assignedLicenses** プロパティは、**assignedLicense** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4b43f-p101">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="4b43f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b43f-104">Properties</span></span>
| <span data-ttu-id="4b43f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b43f-105">Property</span></span>     | <span data-ttu-id="4b43f-106">型</span><span class="sxs-lookup"><span data-stu-id="4b43f-106">Type</span></span>   |<span data-ttu-id="4b43f-107">説明</span><span class="sxs-lookup"><span data-stu-id="4b43f-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b43f-108">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="4b43f-108">disabledPlans</span></span>|<span data-ttu-id="4b43f-109">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="4b43f-109">Guid collection</span></span>|<span data-ttu-id="4b43f-110">無効になっているプランの一意識別子のコレクション。</span><span class="sxs-lookup"><span data-stu-id="4b43f-110">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="4b43f-111">skuId</span><span class="sxs-lookup"><span data-stu-id="4b43f-111">skuId</span></span>|<span data-ttu-id="4b43f-112">Guid</span><span class="sxs-lookup"><span data-stu-id="4b43f-112">Guid</span></span>|<span data-ttu-id="4b43f-113">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4b43f-113">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b43f-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b43f-114">JSON representation</span></span>

<span data-ttu-id="4b43f-115">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4b43f-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
