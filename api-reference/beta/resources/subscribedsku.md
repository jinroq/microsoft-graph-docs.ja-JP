---
title: subscribedSku リソースの種類
description: " 作成、更新、および削除はサポートされていません。 クエリのフィルター式はサポートされていません。 directoryObject から継承します。"
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090e6912ce2f337a8e30322c9b45161af73175cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522701"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="44a37-105">subscribedSku リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44a37-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44a37-p102">購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="44a37-p102">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="44a37-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="44a37-109">Methods</span></span>
| <span data-ttu-id="44a37-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="44a37-110">Method</span></span>           | <span data-ttu-id="44a37-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="44a37-111">Return Type</span></span>    |<span data-ttu-id="44a37-112">説明</span><span class="sxs-lookup"><span data-stu-id="44a37-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44a37-113">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="44a37-113">[Get subscribedSku](../api/subscribedsku-get.md)</span></span> | [<span data-ttu-id="44a37-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="44a37-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="44a37-115">subscribedSku オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="44a37-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="44a37-116">subscribedSku を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="44a37-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="44a37-117">[subscribedSku](subscribedsku.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="44a37-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="44a37-118">組織で取得した商用サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="44a37-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="44a37-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44a37-119">Properties</span></span>
| <span data-ttu-id="44a37-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44a37-120">Property</span></span>     | <span data-ttu-id="44a37-121">型</span><span class="sxs-lookup"><span data-stu-id="44a37-121">Type</span></span>   |<span data-ttu-id="44a37-122">説明</span><span class="sxs-lookup"><span data-stu-id="44a37-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44a37-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="44a37-123">appliesTo</span></span>|<span data-ttu-id="44a37-124">String</span><span class="sxs-lookup"><span data-stu-id="44a37-124">String</span></span>| <span data-ttu-id="44a37-125">"User" や "Company" など。</span><span class="sxs-lookup"><span data-stu-id="44a37-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="44a37-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="44a37-126">capabilityStatus</span></span>|<span data-ttu-id="44a37-127">String</span><span class="sxs-lookup"><span data-stu-id="44a37-127">String</span></span>| <span data-ttu-id="44a37-128">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="44a37-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="44a37-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="44a37-129">consumedUnits</span></span>|<span data-ttu-id="44a37-130">Int32</span><span class="sxs-lookup"><span data-stu-id="44a37-130">Int32</span></span>| <span data-ttu-id="44a37-131">割り当てられたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="44a37-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="44a37-132">id</span><span class="sxs-lookup"><span data-stu-id="44a37-132">id</span></span>|<span data-ttu-id="44a37-133">String</span><span class="sxs-lookup"><span data-stu-id="44a37-133">String</span></span>| <span data-ttu-id="44a37-p103">購読している SKU オブジェクトの一意識別子。キーであり、null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="44a37-p103">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="44a37-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="44a37-136">prepaidUnits</span></span>|[<span data-ttu-id="44a37-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="44a37-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="44a37-138">プリペイド ライセンスの数と状態に関する情報。</span><span class="sxs-lookup"><span data-stu-id="44a37-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="44a37-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="44a37-139">servicePlans</span></span>|<span data-ttu-id="44a37-140">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="44a37-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="44a37-p104">SKU と併用できるサービス プランに関する情報。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="44a37-p104">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="44a37-143">skuId</span><span class="sxs-lookup"><span data-stu-id="44a37-143">skuId</span></span>|<span data-ttu-id="44a37-144">Guid</span><span class="sxs-lookup"><span data-stu-id="44a37-144">Guid</span></span>| <span data-ttu-id="44a37-145">サービス SKU の一意識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="44a37-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="44a37-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="44a37-146">skuPartNumber</span></span>|<span data-ttu-id="44a37-147">String</span><span class="sxs-lookup"><span data-stu-id="44a37-147">String</span></span>| <span data-ttu-id="44a37-148">SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。</span><span class="sxs-lookup"><span data-stu-id="44a37-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="44a37-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="44a37-149">Relationships</span></span>
<span data-ttu-id="44a37-150">なし</span><span class="sxs-lookup"><span data-stu-id="44a37-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44a37-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44a37-151">JSON representation</span></span>

<span data-ttu-id="44a37-152">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="44a37-152">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/subscribedsku.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
