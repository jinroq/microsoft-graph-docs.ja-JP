---
title: governancePermission リソースの種類
description: 'governanceSubject が特定の governanceResource に対して持つアクセス許可を表します。  '
localization_priority: Normal
ms.openlocfilehash: 2f6be4bdc502f829b1dcfd991d1c2ae6130dea8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340183"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="e7e2d-103">governancePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7e2d-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7e2d-104">[governanceSubject](../resources/governancesubject.md)が特定の[governanceResource](../resources/governanceresource.md)に対して持つアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="e7e2d-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="e7e2d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7e2d-105">Properties</span></span>
| <span data-ttu-id="e7e2d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7e2d-106">Property</span></span>     | <span data-ttu-id="e7e2d-107">型</span><span class="sxs-lookup"><span data-stu-id="e7e2d-107">Type</span></span>   |<span data-ttu-id="e7e2d-108">説明</span><span class="sxs-lookup"><span data-stu-id="e7e2d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7e2d-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e7e2d-109">accessLevel</span></span>|<span data-ttu-id="e7e2d-110">String</span><span class="sxs-lookup"><span data-stu-id="e7e2d-110">String</span></span>|<span data-ttu-id="e7e2d-111">アクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="e7e2d-111">The access level.</span></span> <span data-ttu-id="e7e2d-112">有効な値``None``は``UserRead``、 ``AdminRead``、、 ``AdminReadWrite``、です。</span><span class="sxs-lookup"><span data-stu-id="e7e2d-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="e7e2d-113">isActive</span><span class="sxs-lookup"><span data-stu-id="e7e2d-113">isActive</span></span>|<span data-ttu-id="e7e2d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7e2d-114">Boolean</span></span>|<span data-ttu-id="e7e2d-115">要求者がアクセスレベルに対してアクティブなロール割り当てを持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7e2d-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="e7e2d-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="e7e2d-116">isEligible</span></span>|<span data-ttu-id="e7e2d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7e2d-117">Boolean</span></span>|<span data-ttu-id="e7e2d-118">要求者がアクセスレベルに対して適格な役割の割り当てを持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7e2d-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7e2d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7e2d-119">JSON representation</span></span>

<span data-ttu-id="e7e2d-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7e2d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
