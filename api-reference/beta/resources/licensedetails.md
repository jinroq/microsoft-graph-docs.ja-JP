---
title: licenseDetails リソースの種類
description: ユーザーに割り当てられているライセンスに関する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 1f0992904a124931be239fd18ad2bf187e01c41c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885751"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="152f0-103">licenseDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="152f0-103">licenseDetails resource type</span></span>

> <span data-ttu-id="152f0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="152f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="152f0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="152f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="152f0-106">ユーザーに割り当てられているライセンスに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="152f0-106">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="152f0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="152f0-107">Methods</span></span>

| <span data-ttu-id="152f0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="152f0-108">Method</span></span>           | <span data-ttu-id="152f0-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="152f0-109">Return Type</span></span>    |<span data-ttu-id="152f0-110">説明</span><span class="sxs-lookup"><span data-stu-id="152f0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="152f0-111">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="152f0-111">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="152f0-112">licenseDetails コレクション</span><span class="sxs-lookup"><span data-stu-id="152f0-112">licenseDetails collection</span></span> |<span data-ttu-id="152f0-113">ユーザーの licenseDetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="152f0-113">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="152f0-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="152f0-114">Properties</span></span>
| <span data-ttu-id="152f0-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="152f0-115">Property</span></span>     | <span data-ttu-id="152f0-116">種類</span><span class="sxs-lookup"><span data-stu-id="152f0-116">Type</span></span>   |<span data-ttu-id="152f0-117">説明</span><span class="sxs-lookup"><span data-stu-id="152f0-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="152f0-118">ID</span><span class="sxs-lookup"><span data-stu-id="152f0-118">id</span></span>|<span data-ttu-id="152f0-119">String</span><span class="sxs-lookup"><span data-stu-id="152f0-119">String</span></span>| <span data-ttu-id="152f0-p102">ライセンス詳細オブジェクトの一意識別子。読み取り専用。キー。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="152f0-p102">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="152f0-122">servicePlans</span><span class="sxs-lookup"><span data-stu-id="152f0-122">servicePlans</span></span>|<span data-ttu-id="152f0-123">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="152f0-123">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="152f0-p103">ライセンスが割り当てられたサービス プランに関する情報。読み取り専用。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="152f0-p103">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="152f0-126">skuId</span><span class="sxs-lookup"><span data-stu-id="152f0-126">skuId</span></span>|<span data-ttu-id="152f0-127">Guid</span><span class="sxs-lookup"><span data-stu-id="152f0-127">Guid</span></span>| <span data-ttu-id="152f0-p104">サービス SKU の一意識別子 (GUID)。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuId プロパティと同じです。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="152f0-p104">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="152f0-131">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="152f0-131">skuPartNumber</span></span>|<span data-ttu-id="152f0-132">String</span><span class="sxs-lookup"><span data-stu-id="152f0-132">String</span></span>| <span data-ttu-id="152f0-p105">一意の SKU 表示名です。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuPartNumber と同じです。例: "AAD_Premium"。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="152f0-p105">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="152f0-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="152f0-136">Relationships</span></span>
<span data-ttu-id="152f0-137">なし</span><span class="sxs-lookup"><span data-stu-id="152f0-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="152f0-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="152f0-138">JSON representation</span></span>
<span data-ttu-id="152f0-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="152f0-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
