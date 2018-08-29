# <a name="subscribedsku-resource-type"></a><span data-ttu-id="b240e-101">subscribedSku リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b240e-101">subscribedSku resource type</span></span>

<span data-ttu-id="b240e-102">会社が購読しているサービス SKU に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b240e-102">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="b240e-p101">購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="b240e-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b240e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b240e-106">Methods</span></span>
| <span data-ttu-id="b240e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b240e-107">Method</span></span>           | <span data-ttu-id="b240e-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b240e-108">Return Type</span></span>    |<span data-ttu-id="b240e-109">説明</span><span class="sxs-lookup"><span data-stu-id="b240e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b240e-110">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="b240e-110">Get subscribedSku</span></span>](../api/subscribedsku_get.md) | [<span data-ttu-id="b240e-111">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="b240e-111">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="b240e-112">subscribedSku オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b240e-112">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="b240e-113">subscribedSku を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b240e-113">List subscribedSku</span></span>](../api/subscribedsku_list.md) | <span data-ttu-id="b240e-114">[subscribedSku](subscribedsku.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b240e-114">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="b240e-115">組織で取得した商用サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b240e-115">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="b240e-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b240e-116">Properties</span></span>
| <span data-ttu-id="b240e-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b240e-117">Property</span></span>     | <span data-ttu-id="b240e-118">タイプ</span><span class="sxs-lookup"><span data-stu-id="b240e-118">Type</span></span>   |<span data-ttu-id="b240e-119">説明</span><span class="sxs-lookup"><span data-stu-id="b240e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b240e-120">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b240e-120">appliesTo</span></span>|<span data-ttu-id="b240e-121">文字列</span><span class="sxs-lookup"><span data-stu-id="b240e-121">String</span></span>| <span data-ttu-id="b240e-122">"User" や "Company" など。</span><span class="sxs-lookup"><span data-stu-id="b240e-122">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="b240e-123">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="b240e-123">capabilityStatus</span></span>|<span data-ttu-id="b240e-124">文字列</span><span class="sxs-lookup"><span data-stu-id="b240e-124">String</span></span>| <span data-ttu-id="b240e-125">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="b240e-125">For example, "Enabled".</span></span> |
|<span data-ttu-id="b240e-126">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="b240e-126">consumedUnits</span></span>|<span data-ttu-id="b240e-127">Int32</span><span class="sxs-lookup"><span data-stu-id="b240e-127">Int32</span></span>| <span data-ttu-id="b240e-128">割り当てられたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="b240e-128">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="b240e-129">ID</span><span class="sxs-lookup"><span data-stu-id="b240e-129">id</span></span>|<span data-ttu-id="b240e-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b240e-130">String</span></span>| <span data-ttu-id="b240e-p102">購読している SKU オブジェクトの一意識別子。キーであり、null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="b240e-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="b240e-133">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="b240e-133">prepaidUnits</span></span>|[<span data-ttu-id="b240e-134">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="b240e-134">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="b240e-135">プリペイド ライセンスの数と状態に関する情報。</span><span class="sxs-lookup"><span data-stu-id="b240e-135">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="b240e-136">servicePlans</span><span class="sxs-lookup"><span data-stu-id="b240e-136">servicePlans</span></span>|<span data-ttu-id="b240e-137">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b240e-137">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="b240e-p103">SKU と併用できるサービス プランに関する情報。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="b240e-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="b240e-140">skuId</span><span class="sxs-lookup"><span data-stu-id="b240e-140">skuId</span></span>|<span data-ttu-id="b240e-141">Guid</span><span class="sxs-lookup"><span data-stu-id="b240e-141">Guid</span></span>| <span data-ttu-id="b240e-142">サービス SKU の一意識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="b240e-142">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="b240e-143">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="b240e-143">skuPartNumber</span></span>|<span data-ttu-id="b240e-144">文字列</span><span class="sxs-lookup"><span data-stu-id="b240e-144">String</span></span>| <span data-ttu-id="b240e-145">SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。</span><span class="sxs-lookup"><span data-stu-id="b240e-145">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="b240e-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b240e-146">Relationships</span></span>
<span data-ttu-id="b240e-147">なし</span><span class="sxs-lookup"><span data-stu-id="b240e-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b240e-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b240e-148">JSON representation</span></span>

<span data-ttu-id="b240e-149">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b240e-149">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
