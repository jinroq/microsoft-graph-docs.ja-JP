---
title: licensedetails リソースの種類
description: ユーザーに割り当てられているライセンスに関する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 7036904e20173f8fefb6f4f02bd2473289de96c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562679"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="92ac3-103">licensedetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92ac3-103">licenseDetails resource type</span></span>

<span data-ttu-id="92ac3-104">ユーザーに割り当てられているライセンスに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92ac3-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="92ac3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="92ac3-105">Methods</span></span>

| <span data-ttu-id="92ac3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="92ac3-106">Method</span></span>           | <span data-ttu-id="92ac3-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="92ac3-107">Return Type</span></span>    |<span data-ttu-id="92ac3-108">説明</span><span class="sxs-lookup"><span data-stu-id="92ac3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92ac3-109">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="92ac3-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="92ac3-110">licenseDetails コレクション</span><span class="sxs-lookup"><span data-stu-id="92ac3-110">licenseDetails collection</span></span> |<span data-ttu-id="92ac3-111">ユーザーの licensedetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="92ac3-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="92ac3-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92ac3-112">Properties</span></span>
| <span data-ttu-id="92ac3-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92ac3-113">Property</span></span>     | <span data-ttu-id="92ac3-114">型</span><span class="sxs-lookup"><span data-stu-id="92ac3-114">Type</span></span>   |<span data-ttu-id="92ac3-115">説明</span><span class="sxs-lookup"><span data-stu-id="92ac3-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92ac3-116">id</span><span class="sxs-lookup"><span data-stu-id="92ac3-116">id</span></span>|<span data-ttu-id="92ac3-117">String</span><span class="sxs-lookup"><span data-stu-id="92ac3-117">String</span></span>| <span data-ttu-id="92ac3-118">ライセンス詳細オブジェクトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="92ac3-118">The unique identifier for the license detail object.</span></span> <span data-ttu-id="92ac3-119">読み取り専用、キー、null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="92ac3-119">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="92ac3-120">serviceplans</span><span class="sxs-lookup"><span data-stu-id="92ac3-120">servicePlans</span></span>|<span data-ttu-id="92ac3-121">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92ac3-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="92ac3-122">ライセンスで割り当てられているサービスプランに関する情報。</span><span class="sxs-lookup"><span data-stu-id="92ac3-122">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="92ac3-123">読み取り専用で、null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="92ac3-123">Read-only, Not nullable</span></span> |
|<span data-ttu-id="92ac3-124">skuId</span><span class="sxs-lookup"><span data-stu-id="92ac3-124">skuId</span></span>|<span data-ttu-id="92ac3-125">Guid</span><span class="sxs-lookup"><span data-stu-id="92ac3-125">Guid</span></span>| <span data-ttu-id="92ac3-126">サービス SKU の一意識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="92ac3-126">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="92ac3-127">関連する[SubscribedSku](subscribedsku.md)オブジェクトの skuId プロパティと同じです。</span><span class="sxs-lookup"><span data-stu-id="92ac3-127">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="92ac3-128">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="92ac3-128">Read-only</span></span> |
|<span data-ttu-id="92ac3-129">skupartnumber</span><span class="sxs-lookup"><span data-stu-id="92ac3-129">skuPartNumber</span></span>|<span data-ttu-id="92ac3-130">String</span><span class="sxs-lookup"><span data-stu-id="92ac3-130">String</span></span>| <span data-ttu-id="92ac3-131">一意の SKU 表示名。</span><span class="sxs-lookup"><span data-stu-id="92ac3-131">Unique SKU display name.</span></span> <span data-ttu-id="92ac3-132">関連する[SubscribedSku](subscribedsku.md)オブジェクトの skupartnumber と等しい。例: "AAD_Premium"。</span><span class="sxs-lookup"><span data-stu-id="92ac3-132">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="92ac3-133">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="92ac3-133">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="92ac3-134">関係</span><span class="sxs-lookup"><span data-stu-id="92ac3-134">Relationships</span></span>
<span data-ttu-id="92ac3-135">なし</span><span class="sxs-lookup"><span data-stu-id="92ac3-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92ac3-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92ac3-136">JSON representation</span></span>
<span data-ttu-id="92ac3-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92ac3-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
