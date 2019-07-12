---
title: subscribedSku リソースの種類
description: " create、update、および delete はサポートされていません。 クエリのフィルター式はサポートされていません。 directoryObject から継承します。"
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c2bca99fed2b8c5328c2f2cf1ac3bf938ddcfcaa
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639025"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="c2251-105">subscribedSku リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c2251-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2251-p102">購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="c2251-p102">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="c2251-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c2251-109">Methods</span></span>
| <span data-ttu-id="c2251-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c2251-110">Method</span></span>           | <span data-ttu-id="c2251-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c2251-111">Return Type</span></span>    |<span data-ttu-id="c2251-112">説明</span><span class="sxs-lookup"><span data-stu-id="c2251-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2251-113">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="c2251-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="c2251-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c2251-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="c2251-115">組織が取得した特定の商用サブスクリプションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c2251-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="c2251-116">リスト subscribedsku</span><span class="sxs-lookup"><span data-stu-id="c2251-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="c2251-117">[subscribedSku](subscribedsku.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c2251-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="c2251-118">組織が取得した商用サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c2251-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2251-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2251-119">Properties</span></span>
| <span data-ttu-id="c2251-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2251-120">Property</span></span>     | <span data-ttu-id="c2251-121">型</span><span class="sxs-lookup"><span data-stu-id="c2251-121">Type</span></span>   |<span data-ttu-id="c2251-122">説明</span><span class="sxs-lookup"><span data-stu-id="c2251-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2251-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="c2251-123">appliesTo</span></span>|<span data-ttu-id="c2251-124">String</span><span class="sxs-lookup"><span data-stu-id="c2251-124">String</span></span>| <span data-ttu-id="c2251-125">"User" や "Company" など。</span><span class="sxs-lookup"><span data-stu-id="c2251-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="c2251-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="c2251-126">capabilityStatus</span></span>|<span data-ttu-id="c2251-127">String</span><span class="sxs-lookup"><span data-stu-id="c2251-127">String</span></span>| <span data-ttu-id="c2251-128">たとえば、"有効" です。</span><span class="sxs-lookup"><span data-stu-id="c2251-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="c2251-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="c2251-129">consumedUnits</span></span>|<span data-ttu-id="c2251-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c2251-130">Int32</span></span>| <span data-ttu-id="c2251-131">割り当てられたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="c2251-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="c2251-132">id</span><span class="sxs-lookup"><span data-stu-id="c2251-132">id</span></span>|<span data-ttu-id="c2251-133">String</span><span class="sxs-lookup"><span data-stu-id="c2251-133">String</span></span>| <span data-ttu-id="c2251-134">購読している SKU オブジェクトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c2251-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="c2251-135">キー。 null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="c2251-135">Key, not nullable.</span></span> |
|<span data-ttu-id="c2251-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="c2251-136">prepaidUnits</span></span>|[<span data-ttu-id="c2251-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="c2251-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="c2251-138">プリペイド ライセンスの数と状態に関する情報。</span><span class="sxs-lookup"><span data-stu-id="c2251-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="c2251-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="c2251-139">servicePlans</span></span>|<span data-ttu-id="c2251-140">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c2251-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="c2251-141">SKU と併用できるサービス プランに関する情報。</span><span class="sxs-lookup"><span data-stu-id="c2251-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="c2251-142">Null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="c2251-142">Not nullable</span></span> |
|<span data-ttu-id="c2251-143">skuId</span><span class="sxs-lookup"><span data-stu-id="c2251-143">skuId</span></span>|<span data-ttu-id="c2251-144">Guid</span><span class="sxs-lookup"><span data-stu-id="c2251-144">Guid</span></span>| <span data-ttu-id="c2251-145">サービス SKU の一意識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="c2251-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="c2251-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="c2251-146">skuPartNumber</span></span>|<span data-ttu-id="c2251-147">String</span><span class="sxs-lookup"><span data-stu-id="c2251-147">String</span></span>| <span data-ttu-id="c2251-148">SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。</span><span class="sxs-lookup"><span data-stu-id="c2251-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="c2251-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c2251-149">Relationships</span></span>
<span data-ttu-id="c2251-150">なし</span><span class="sxs-lookup"><span data-stu-id="c2251-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2251-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c2251-151">JSON representation</span></span>

<span data-ttu-id="c2251-152">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c2251-152">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
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
<!--
{
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
