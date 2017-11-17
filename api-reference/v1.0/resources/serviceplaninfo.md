# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="ece5f-101">servicePlanInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ece5f-101">servicePlanInfo resource type</span></span>

<span data-ttu-id="ece5f-p101">購読している SKU に関連付けられているサービス プランに関する情報が含まれています。[subscribedSku](subscribedsku.md) エンティティの **servicePlans** プロパティは、**servicePlanInfo** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ece5f-p101">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="ece5f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ece5f-104">Properties</span></span>
| <span data-ttu-id="ece5f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ece5f-105">Property</span></span>     | <span data-ttu-id="ece5f-106">型</span><span class="sxs-lookup"><span data-stu-id="ece5f-106">Type</span></span>   |<span data-ttu-id="ece5f-107">説明</span><span class="sxs-lookup"><span data-stu-id="ece5f-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ece5f-108">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="ece5f-108">servicePlanId</span></span>|<span data-ttu-id="ece5f-109">Guid</span><span class="sxs-lookup"><span data-stu-id="ece5f-109">Guid</span></span>|<span data-ttu-id="ece5f-110">サービス プランの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ece5f-110">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="ece5f-111">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="ece5f-111">servicePlanName</span></span>|<span data-ttu-id="ece5f-112">String</span><span class="sxs-lookup"><span data-stu-id="ece5f-112">String</span></span>|<span data-ttu-id="ece5f-113">サービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="ece5f-113">The name of the service plan.</span></span>|
|<span data-ttu-id="ece5f-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="ece5f-114">provisioningStatus</span></span>|<span data-ttu-id="ece5f-115">String</span><span class="sxs-lookup"><span data-stu-id="ece5f-115">String</span></span>|<span data-ttu-id="ece5f-p102">サービス プランのプロビジョニング状況。可能な値:</span><span class="sxs-lookup"><span data-stu-id="ece5f-p102">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="ece5f-118">Success - サービスは完全にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="ece5f-118">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="ece5f-119">Disabled - サービスは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="ece5f-119">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="ece5f-120">PendingInput - サービスはまだプロビジョニングされていません。サービスの確認を待っています。</span><span class="sxs-lookup"><span data-stu-id="ece5f-120">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="ece5f-121">PendingActivation - サービスはプロビジョニングされていますが、管理者による明示的なアクティブ化が必要です (Intune_O365 サービスプランなど)</span><span class="sxs-lookup"><span data-stu-id="ece5f-121">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="ece5f-122">PendingProvisioning - Microsoft では製品の SKU に新しいサービスを追加していますが、テナント側でまだアクティブ化されていません。</span><span class="sxs-lookup"><span data-stu-id="ece5f-122">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="ece5f-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="ece5f-123">appliesTo</span></span>|<span data-ttu-id="ece5f-124">String</span><span class="sxs-lookup"><span data-stu-id="ece5f-124">String</span></span>|<span data-ttu-id="ece5f-p103">サービス プランを割り当てることができるオブジェクト。可能な値:</span><span class="sxs-lookup"><span data-stu-id="ece5f-p103">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="ece5f-127">User - サービス プランを個別のユーザーに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="ece5f-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="ece5f-128">Company - サービス プランをテナント全体に割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="ece5f-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ece5f-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ece5f-129">JSON representation</span></span>

<span data-ttu-id="ece5f-130">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ece5f-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
