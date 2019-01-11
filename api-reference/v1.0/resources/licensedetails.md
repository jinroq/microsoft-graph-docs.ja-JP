---
title: licenseDetails リソースの種類
description: ユーザーに割り当てられているライセンスに関する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 4495e85b45f6fcfda4f37e467e9cdc5393787dc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843023"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="e88c6-103">licenseDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e88c6-103">licenseDetails resource type</span></span>

<span data-ttu-id="e88c6-104">ユーザーに割り当てられているライセンスに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e88c6-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="e88c6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e88c6-105">Methods</span></span>

| <span data-ttu-id="e88c6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e88c6-106">Method</span></span>           | <span data-ttu-id="e88c6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e88c6-107">Return Type</span></span>    |<span data-ttu-id="e88c6-108">説明</span><span class="sxs-lookup"><span data-stu-id="e88c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e88c6-109">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e88c6-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="e88c6-110">licenseDetails コレクション</span><span class="sxs-lookup"><span data-stu-id="e88c6-110">licenseDetails collection</span></span> |<span data-ttu-id="e88c6-111">ユーザーの licenseDetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e88c6-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="e88c6-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e88c6-112">Properties</span></span>
| <span data-ttu-id="e88c6-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e88c6-113">Property</span></span>     | <span data-ttu-id="e88c6-114">種類</span><span class="sxs-lookup"><span data-stu-id="e88c6-114">Type</span></span>   |<span data-ttu-id="e88c6-115">説明</span><span class="sxs-lookup"><span data-stu-id="e88c6-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e88c6-116">ID</span><span class="sxs-lookup"><span data-stu-id="e88c6-116">id</span></span>|<span data-ttu-id="e88c6-117">String</span><span class="sxs-lookup"><span data-stu-id="e88c6-117">String</span></span>| <span data-ttu-id="e88c6-p101">ライセンス詳細オブジェクトの一意識別子。読み取り専用。キー。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="e88c6-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="e88c6-120">servicePlans</span><span class="sxs-lookup"><span data-stu-id="e88c6-120">servicePlans</span></span>|<span data-ttu-id="e88c6-121">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e88c6-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="e88c6-p102">ライセンスが割り当てられたサービス プランに関する情報。読み取り専用。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="e88c6-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="e88c6-124">skuId</span><span class="sxs-lookup"><span data-stu-id="e88c6-124">skuId</span></span>|<span data-ttu-id="e88c6-125">Guid</span><span class="sxs-lookup"><span data-stu-id="e88c6-125">Guid</span></span>| <span data-ttu-id="e88c6-p103">サービス SKU の一意識別子 (GUID)。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuId プロパティと同じです。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="e88c6-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="e88c6-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="e88c6-129">skuPartNumber</span></span>|<span data-ttu-id="e88c6-130">String</span><span class="sxs-lookup"><span data-stu-id="e88c6-130">String</span></span>| <span data-ttu-id="e88c6-p104">一意の SKU 表示名です。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuPartNumber と同じです。例: "AAD_Premium"。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="e88c6-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="e88c6-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e88c6-134">Relationships</span></span>
<span data-ttu-id="e88c6-135">なし</span><span class="sxs-lookup"><span data-stu-id="e88c6-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e88c6-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e88c6-136">JSON representation</span></span>
<span data-ttu-id="e88c6-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e88c6-137">Here is a JSON representation of the resource.</span></span>

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
