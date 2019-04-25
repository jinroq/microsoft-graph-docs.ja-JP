---
title: assignedLicense リソースの種類
description: ユーザーに割り当てられているライセンスを表します。 user エンティティの**assignedLicenses**プロパティは、 **assignedLicense**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 2d9620ec33a296c09ced9bc9d8af8d6d032bb7d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535656"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="abee8-104">assignedLicense リソースの種類</span><span class="sxs-lookup"><span data-stu-id="abee8-104">assignedLicense resource type</span></span>

<span data-ttu-id="abee8-105">ユーザーに割り当てられているライセンスを表します。</span><span class="sxs-lookup"><span data-stu-id="abee8-105">Represents a license assigned to a user.</span></span> <span data-ttu-id="abee8-106">[user](user.md)エンティティの**assignedLicenses**プロパティは、 **assignedLicense**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="abee8-106">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="abee8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abee8-107">Properties</span></span>
| <span data-ttu-id="abee8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abee8-108">Property</span></span>     | <span data-ttu-id="abee8-109">型</span><span class="sxs-lookup"><span data-stu-id="abee8-109">Type</span></span>   |<span data-ttu-id="abee8-110">説明</span><span class="sxs-lookup"><span data-stu-id="abee8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abee8-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="abee8-111">disabledPlans</span></span>|<span data-ttu-id="abee8-112">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="abee8-112">Guid collection</span></span>|<span data-ttu-id="abee8-113">無効になっているプランの一意識別子のコレクション。</span><span class="sxs-lookup"><span data-stu-id="abee8-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="abee8-114">skuId</span><span class="sxs-lookup"><span data-stu-id="abee8-114">skuId</span></span>|<span data-ttu-id="abee8-115">Guid</span><span class="sxs-lookup"><span data-stu-id="abee8-115">Guid</span></span>|<span data-ttu-id="abee8-116">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="abee8-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abee8-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="abee8-117">JSON representation</span></span>

<span data-ttu-id="abee8-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="abee8-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
