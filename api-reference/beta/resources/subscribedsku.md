---
title: subscribedSku リソースの種類
description: " 作成、更新、および削除はサポートされていません。 クエリのフィルター式はサポートされていません。 directoryObject から継承します。"
localization_priority: Normal
ms.openlocfilehash: 07f40c766d7f46974cf99b9954f63a61c2c0c621
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829604"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="1b51f-105">subscribedSku リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1b51f-105">subscribedSku resource type</span></span>

> <span data-ttu-id="1b51f-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1b51f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b51f-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b51f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b51f-p103">購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="1b51f-p103">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="1b51f-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="1b51f-111">Methods</span></span>
| <span data-ttu-id="1b51f-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="1b51f-112">Method</span></span>           | <span data-ttu-id="1b51f-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1b51f-113">Return Type</span></span>    |<span data-ttu-id="1b51f-114">説明</span><span class="sxs-lookup"><span data-stu-id="1b51f-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b51f-115">subscribedSku を取得する</span><span class="sxs-lookup"><span data-stu-id="1b51f-115">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="1b51f-116">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="1b51f-116">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="1b51f-117">subscribedSku オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1b51f-117">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="1b51f-118">リスト subscribedsku</span><span class="sxs-lookup"><span data-stu-id="1b51f-118">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="1b51f-119">[subscribedSku](subscribedsku.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1b51f-119">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="1b51f-120">組織で取得した商用サブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1b51f-120">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b51f-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b51f-121">Properties</span></span>
| <span data-ttu-id="1b51f-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b51f-122">Property</span></span>     | <span data-ttu-id="1b51f-123">種類</span><span class="sxs-lookup"><span data-stu-id="1b51f-123">Type</span></span>   |<span data-ttu-id="1b51f-124">説明</span><span class="sxs-lookup"><span data-stu-id="1b51f-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b51f-125">appliesTo</span><span class="sxs-lookup"><span data-stu-id="1b51f-125">appliesTo</span></span>|<span data-ttu-id="1b51f-126">String</span><span class="sxs-lookup"><span data-stu-id="1b51f-126">String</span></span>| <span data-ttu-id="1b51f-127">"User" や "Company" など。</span><span class="sxs-lookup"><span data-stu-id="1b51f-127">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="1b51f-128">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="1b51f-128">capabilityStatus</span></span>|<span data-ttu-id="1b51f-129">String</span><span class="sxs-lookup"><span data-stu-id="1b51f-129">String</span></span>| <span data-ttu-id="1b51f-130">「有効」など。</span><span class="sxs-lookup"><span data-stu-id="1b51f-130">For example, "Enabled".</span></span> |
|<span data-ttu-id="1b51f-131">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="1b51f-131">consumedUnits</span></span>|<span data-ttu-id="1b51f-132">Int32</span><span class="sxs-lookup"><span data-stu-id="1b51f-132">Int32</span></span>| <span data-ttu-id="1b51f-133">割り当てられたライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="1b51f-133">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="1b51f-134">id</span><span class="sxs-lookup"><span data-stu-id="1b51f-134">id</span></span>|<span data-ttu-id="1b51f-135">String</span><span class="sxs-lookup"><span data-stu-id="1b51f-135">String</span></span>| <span data-ttu-id="1b51f-p104">購読している SKU オブジェクトの一意識別子。キーであり、null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="1b51f-p104">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="1b51f-138">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="1b51f-138">prepaidUnits</span></span>|[<span data-ttu-id="1b51f-139">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="1b51f-139">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="1b51f-140">プリペイド ライセンスの数と状態に関する情報。</span><span class="sxs-lookup"><span data-stu-id="1b51f-140">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="1b51f-141">servicePlans</span><span class="sxs-lookup"><span data-stu-id="1b51f-141">servicePlans</span></span>|<span data-ttu-id="1b51f-142">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1b51f-142">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="1b51f-p105">SKU と併用できるサービス プランに関する情報。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="1b51f-p105">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="1b51f-145">skuId</span><span class="sxs-lookup"><span data-stu-id="1b51f-145">skuId</span></span>|<span data-ttu-id="1b51f-146">Guid</span><span class="sxs-lookup"><span data-stu-id="1b51f-146">Guid</span></span>| <span data-ttu-id="1b51f-147">サービス SKU の一意識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="1b51f-147">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="1b51f-148">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="1b51f-148">skuPartNumber</span></span>|<span data-ttu-id="1b51f-149">String</span><span class="sxs-lookup"><span data-stu-id="1b51f-149">String</span></span>| <span data-ttu-id="1b51f-150">SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。</span><span class="sxs-lookup"><span data-stu-id="1b51f-150">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="1b51f-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1b51f-151">Relationships</span></span>
<span data-ttu-id="1b51f-152">なし</span><span class="sxs-lookup"><span data-stu-id="1b51f-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b51f-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1b51f-153">JSON representation</span></span>

<span data-ttu-id="1b51f-154">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1b51f-154">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
