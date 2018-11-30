---
title: subscribedSku リソースの種類
description: 会社が購読しているサービス SKU に関する情報が含まれています。
ms.openlocfilehash: 5a3c3515d4d902810db32acf10b4cee6a889bfc9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023034"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="b7a03-103">subscribedSku リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7a03-103">subscribedSku resource type</span></span>

<span data-ttu-id="b7a03-104">会社が購読しているサービス SKU に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7a03-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="b7a03-p101">購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="b7a03-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b7a03-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b7a03-108">Methods</span></span>
| <span data-ttu-id="b7a03-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b7a03-109">Method</span></span>           | <span data-ttu-id="b7a03-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b7a03-110">Return Type</span></span>    |<span data-ttu-id="b7a03-111">説明</span><span class="sxs-lookup"><span data-stu-id="b7a03-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7a03-112">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="b7a03-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="b7a03-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="b7a03-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="b7a03-114">subscribedSku オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b7a03-114">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="b7a03-115">リスト subscribedsku</span><span class="sxs-lookup"><span data-stu-id="b7a03-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="b7a03-116">[subscribedSku](subscribedsku.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b7a03-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="b7a03-117">組織で取得した商用サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b7a03-117">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7a03-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7a03-118">Properties</span></span>
| <span data-ttu-id="b7a03-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7a03-119">Property</span></span>     | <span data-ttu-id="b7a03-120">型</span><span class="sxs-lookup"><span data-stu-id="b7a03-120">Type</span></span>   |<span data-ttu-id="b7a03-121">説明</span><span class="sxs-lookup"><span data-stu-id="b7a03-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7a03-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b7a03-122">appliesTo</span></span>|<span data-ttu-id="b7a03-123">String</span><span class="sxs-lookup"><span data-stu-id="b7a03-123">String</span></span>| <span data-ttu-id="b7a03-124">"User" や "Company" など。</span><span class="sxs-lookup"><span data-stu-id="b7a03-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="b7a03-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="b7a03-125">capabilityStatus</span></span>|<span data-ttu-id="b7a03-126">String</span><span class="sxs-lookup"><span data-stu-id="b7a03-126">String</span></span>| <span data-ttu-id="b7a03-127">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="b7a03-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="b7a03-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="b7a03-128">consumedUnits</span></span>|<span data-ttu-id="b7a03-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b7a03-129">Int32</span></span>| <span data-ttu-id="b7a03-130">割り当てられたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="b7a03-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="b7a03-131">id</span><span class="sxs-lookup"><span data-stu-id="b7a03-131">id</span></span>|<span data-ttu-id="b7a03-132">String</span><span class="sxs-lookup"><span data-stu-id="b7a03-132">String</span></span>| <span data-ttu-id="b7a03-p102">購読している SKU オブジェクトの一意識別子。キーであり、null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="b7a03-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="b7a03-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="b7a03-135">prepaidUnits</span></span>|[<span data-ttu-id="b7a03-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="b7a03-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="b7a03-137">プリペイド ライセンスの数と状態に関する情報。</span><span class="sxs-lookup"><span data-stu-id="b7a03-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="b7a03-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="b7a03-138">servicePlans</span></span>|<span data-ttu-id="b7a03-139">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b7a03-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="b7a03-p103">SKU と併用できるサービス プランに関する情報。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="b7a03-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="b7a03-142">skuId</span><span class="sxs-lookup"><span data-stu-id="b7a03-142">skuId</span></span>|<span data-ttu-id="b7a03-143">Guid</span><span class="sxs-lookup"><span data-stu-id="b7a03-143">Guid</span></span>| <span data-ttu-id="b7a03-144">サービス SKU の一意識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="b7a03-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="b7a03-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="b7a03-145">skuPartNumber</span></span>|<span data-ttu-id="b7a03-146">String</span><span class="sxs-lookup"><span data-stu-id="b7a03-146">String</span></span>| <span data-ttu-id="b7a03-147">SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。</span><span class="sxs-lookup"><span data-stu-id="b7a03-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="b7a03-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7a03-148">Relationships</span></span>
<span data-ttu-id="b7a03-149">なし</span><span class="sxs-lookup"><span data-stu-id="b7a03-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7a03-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7a03-150">JSON representation</span></span>

<span data-ttu-id="b7a03-151">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b7a03-151">Here is a JSON representation of the resource</span></span>

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
