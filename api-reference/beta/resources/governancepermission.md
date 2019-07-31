---
title: governancePermission リソースの種類
description: 'GovernanceSubject が特定の governanceResource に対して持つアクセス許可を表します。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8bf32b855ed77ccdf712b1a739ef913d0a3dade0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971944"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="2069d-103">governancePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2069d-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2069d-104">[GovernanceSubject](../resources/governancesubject.md)が特定の[governanceResource](../resources/governanceresource.md)に対して持つアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="2069d-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="2069d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2069d-105">Properties</span></span>
| <span data-ttu-id="2069d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2069d-106">Property</span></span>     | <span data-ttu-id="2069d-107">型</span><span class="sxs-lookup"><span data-stu-id="2069d-107">Type</span></span>   |<span data-ttu-id="2069d-108">説明</span><span class="sxs-lookup"><span data-stu-id="2069d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2069d-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="2069d-109">accessLevel</span></span>|<span data-ttu-id="2069d-110">String</span><span class="sxs-lookup"><span data-stu-id="2069d-110">String</span></span>|<span data-ttu-id="2069d-111">アクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="2069d-111">The access level.</span></span> <span data-ttu-id="2069d-112">有効な値``None``は``UserRead``、 ``AdminRead``、、 ``AdminReadWrite``、です。</span><span class="sxs-lookup"><span data-stu-id="2069d-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="2069d-113">isActive</span><span class="sxs-lookup"><span data-stu-id="2069d-113">isActive</span></span>|<span data-ttu-id="2069d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="2069d-114">Boolean</span></span>|<span data-ttu-id="2069d-115">要求者がアクセスレベルに対してアクティブなロール割り当てを持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2069d-115">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="2069d-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="2069d-116">isEligible</span></span>|<span data-ttu-id="2069d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="2069d-117">Boolean</span></span>|<span data-ttu-id="2069d-118">要求者がアクセスレベルに対して適格な役割の割り当てを持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2069d-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2069d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2069d-119">JSON representation</span></span>

<span data-ttu-id="2069d-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2069d-120">Here is a JSON representation of the resource.</span></span>
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
