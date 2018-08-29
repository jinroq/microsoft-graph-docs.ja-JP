# <a name="provisionedplan-resource-type"></a><span data-ttu-id="837cc-101">provisionedPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="837cc-101">provisionedPlan resource type</span></span>

<span data-ttu-id="837cc-102">[ユーザー](user.md) エンティティと[組織](organization.md)エンティティの **provisionedPlans** プロパティは、**provisionedPlan** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="837cc-102">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="837cc-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="837cc-103">Properties</span></span>
| <span data-ttu-id="837cc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="837cc-104">Property</span></span>     | <span data-ttu-id="837cc-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="837cc-105">Type</span></span>   |<span data-ttu-id="837cc-106">説明</span><span class="sxs-lookup"><span data-stu-id="837cc-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="837cc-107">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="837cc-107">capabilityStatus</span></span>|<span data-ttu-id="837cc-108">String</span><span class="sxs-lookup"><span data-stu-id="837cc-108">String</span></span>|<span data-ttu-id="837cc-109">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="837cc-109">For example, “Enabled”.</span></span>|
|<span data-ttu-id="837cc-110">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="837cc-110">provisioningStatus</span></span>|<span data-ttu-id="837cc-111">String</span><span class="sxs-lookup"><span data-stu-id="837cc-111">String</span></span>|<span data-ttu-id="837cc-112">「成功」など。</span><span class="sxs-lookup"><span data-stu-id="837cc-112">For example, “Success”.</span></span>|
|<span data-ttu-id="837cc-113">service</span><span class="sxs-lookup"><span data-stu-id="837cc-113">service</span></span>|<span data-ttu-id="837cc-114">String</span><span class="sxs-lookup"><span data-stu-id="837cc-114">String</span></span>|<span data-ttu-id="837cc-115">サービスの名前。「AccessControlS2S」など。</span><span class="sxs-lookup"><span data-stu-id="837cc-115">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="837cc-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="837cc-116">JSON representation</span></span>

<span data-ttu-id="837cc-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="837cc-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->