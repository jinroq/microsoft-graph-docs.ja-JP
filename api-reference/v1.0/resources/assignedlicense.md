---
title: assignedLicense リソースの種類
description: ユーザーに割り当てられているライセンスを表します。ユーザー エンティティの **assignedLicenses** プロパティは、**assignedLicense** のコレクションです。
ms.openlocfilehash: 48863a9acdcfa173a3f0c1a2a008516360ffdf9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021350"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="3232e-104">assignedLicense リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3232e-104">assignedLicense resource type</span></span>

<span data-ttu-id="3232e-p102">ユーザーに割り当てられているライセンスを表します。[ユーザー](user.md) エンティティの **assignedLicenses** プロパティは、**assignedLicense** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="3232e-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="3232e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3232e-107">Properties</span></span>
| <span data-ttu-id="3232e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3232e-108">Property</span></span>     | <span data-ttu-id="3232e-109">型</span><span class="sxs-lookup"><span data-stu-id="3232e-109">Type</span></span>   |<span data-ttu-id="3232e-110">説明</span><span class="sxs-lookup"><span data-stu-id="3232e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3232e-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="3232e-111">disabledPlans</span></span>|<span data-ttu-id="3232e-112">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="3232e-112">Guid collection</span></span>|<span data-ttu-id="3232e-113">無効になっているプランの一意識別子のコレクション。</span><span class="sxs-lookup"><span data-stu-id="3232e-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="3232e-114">skuId</span><span class="sxs-lookup"><span data-stu-id="3232e-114">skuId</span></span>|<span data-ttu-id="3232e-115">Guid</span><span class="sxs-lookup"><span data-stu-id="3232e-115">Guid</span></span>|<span data-ttu-id="3232e-116">SKU の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3232e-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3232e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3232e-117">JSON representation</span></span>

<span data-ttu-id="3232e-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3232e-118">Here is a JSON representation of the resource</span></span>

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
