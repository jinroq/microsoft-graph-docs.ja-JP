---
title: governancePermission リソースの種類
description: 'GovernanceSubject が特定の governanceResource に対して持つアクセス許可を表します。  '
localization_priority: Normal
ms.openlocfilehash: cd5b15a85dee7a193962a6072bcdf34b1d4f131a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621306"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="e2eb9-103">governancePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2eb9-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2eb9-104">[GovernanceSubject](../resources/governancesubject.md)が特定の[governanceResource](../resources/governanceresource.md)に対して持つアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="e2eb9-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="e2eb9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2eb9-105">Properties</span></span>
| <span data-ttu-id="e2eb9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2eb9-106">Property</span></span>     | <span data-ttu-id="e2eb9-107">型</span><span class="sxs-lookup"><span data-stu-id="e2eb9-107">Type</span></span>   |<span data-ttu-id="e2eb9-108">説明</span><span class="sxs-lookup"><span data-stu-id="e2eb9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2eb9-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e2eb9-109">accessLevel</span></span>|<span data-ttu-id="e2eb9-110">String</span><span class="sxs-lookup"><span data-stu-id="e2eb9-110">String</span></span>|<span data-ttu-id="e2eb9-111">アクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="e2eb9-111">The access level.</span></span> <span data-ttu-id="e2eb9-112">有効な値``None``は``UserRead``、 ``AdminRead``、、 ``AdminReadWrite``、です。</span><span class="sxs-lookup"><span data-stu-id="e2eb9-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="e2eb9-113">isActive</span><span class="sxs-lookup"><span data-stu-id="e2eb9-113">isActive</span></span>|<span data-ttu-id="e2eb9-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2eb9-114">Boolean</span></span>|<span data-ttu-id="e2eb9-115">要求者がアクセスレベルに対してアクティブなロール割り当てを持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e2eb9-115">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="e2eb9-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="e2eb9-116">isEligible</span></span>|<span data-ttu-id="e2eb9-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2eb9-117">Boolean</span></span>|<span data-ttu-id="e2eb9-118">要求者がアクセスレベルに対して適格な役割の割り当てを持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e2eb9-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2eb9-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2eb9-119">JSON representation</span></span>

<span data-ttu-id="e2eb9-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2eb9-120">Here is a JSON representation of the resource.</span></span>
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
