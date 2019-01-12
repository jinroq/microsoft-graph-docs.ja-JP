---
title: subscribedSku リソースの種類
description: 会社が購読しているサービス SKU に関する情報が含まれています。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9e61fba199d6d3e509700fe61e75bde240c7f16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937440"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="09373-103">subscribedSku リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09373-103">subscribedSku resource type</span></span>

<span data-ttu-id="09373-104">会社が購読しているサービス SKU に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="09373-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="09373-p101">購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="09373-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="09373-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="09373-108">Methods</span></span>
| <span data-ttu-id="09373-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="09373-109">Method</span></span>           | <span data-ttu-id="09373-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="09373-110">Return Type</span></span>    |<span data-ttu-id="09373-111">説明</span><span class="sxs-lookup"><span data-stu-id="09373-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09373-112">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="09373-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="09373-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="09373-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="09373-114">subscribedSku オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="09373-114">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="09373-115">リスト subscribedsku</span><span class="sxs-lookup"><span data-stu-id="09373-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="09373-116">[subscribedSku](subscribedsku.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="09373-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="09373-117">組織で取得した商用サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="09373-117">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="09373-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09373-118">Properties</span></span>
| <span data-ttu-id="09373-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09373-119">Property</span></span>     | <span data-ttu-id="09373-120">型</span><span class="sxs-lookup"><span data-stu-id="09373-120">Type</span></span>   |<span data-ttu-id="09373-121">説明</span><span class="sxs-lookup"><span data-stu-id="09373-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09373-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="09373-122">appliesTo</span></span>|<span data-ttu-id="09373-123">String</span><span class="sxs-lookup"><span data-stu-id="09373-123">String</span></span>| <span data-ttu-id="09373-124">"User" や "Company" など。</span><span class="sxs-lookup"><span data-stu-id="09373-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="09373-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="09373-125">capabilityStatus</span></span>|<span data-ttu-id="09373-126">String</span><span class="sxs-lookup"><span data-stu-id="09373-126">String</span></span>| <span data-ttu-id="09373-127">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="09373-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="09373-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="09373-128">consumedUnits</span></span>|<span data-ttu-id="09373-129">Int32</span><span class="sxs-lookup"><span data-stu-id="09373-129">Int32</span></span>| <span data-ttu-id="09373-130">割り当てられたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="09373-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="09373-131">id</span><span class="sxs-lookup"><span data-stu-id="09373-131">id</span></span>|<span data-ttu-id="09373-132">String</span><span class="sxs-lookup"><span data-stu-id="09373-132">String</span></span>| <span data-ttu-id="09373-p102">購読している SKU オブジェクトの一意識別子。キーであり、null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="09373-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="09373-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="09373-135">prepaidUnits</span></span>|[<span data-ttu-id="09373-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="09373-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="09373-137">プリペイド ライセンスの数と状態に関する情報。</span><span class="sxs-lookup"><span data-stu-id="09373-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="09373-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="09373-138">servicePlans</span></span>|<span data-ttu-id="09373-139">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="09373-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="09373-p103">SKU と併用できるサービス プランに関する情報。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="09373-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="09373-142">skuId</span><span class="sxs-lookup"><span data-stu-id="09373-142">skuId</span></span>|<span data-ttu-id="09373-143">Guid</span><span class="sxs-lookup"><span data-stu-id="09373-143">Guid</span></span>| <span data-ttu-id="09373-144">サービス SKU の一意識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="09373-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="09373-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="09373-145">skuPartNumber</span></span>|<span data-ttu-id="09373-146">String</span><span class="sxs-lookup"><span data-stu-id="09373-146">String</span></span>| <span data-ttu-id="09373-147">SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。</span><span class="sxs-lookup"><span data-stu-id="09373-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="09373-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09373-148">Relationships</span></span>
<span data-ttu-id="09373-149">なし</span><span class="sxs-lookup"><span data-stu-id="09373-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09373-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09373-150">JSON representation</span></span>

<span data-ttu-id="09373-151">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="09373-151">Here is a JSON representation of the resource</span></span>

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
