---
title: targetResourcePolicy リソースの種類
description: '監査活動によって影響を与えたのポリシーを示します。 TargetResource リソースから派生します。   '
localization_priority: Normal
ms.openlocfilehash: 355e6ac11741a2aa7aeb780bdac4b7be373092af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813140"
---
# <a name="targetresourcepolicy-resource-type"></a><span data-ttu-id="c14e8-104">targetResourcePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c14e8-104">targetResourcePolicy resource type</span></span>
<span data-ttu-id="c14e8-105">監査活動によって影響を与えたのポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="c14e8-105">Indicates the policy that was impacted by the audit activity.</span></span> <span data-ttu-id="c14e8-106">[TargetResource](targetresource.md)リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="c14e8-106">Derived from the [targetResource](targetresource.md) resource.</span></span>   



## <a name="properties"></a><span data-ttu-id="c14e8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c14e8-107">Properties</span></span>
| <span data-ttu-id="c14e8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c14e8-108">Property</span></span>     | <span data-ttu-id="c14e8-109">種類</span><span class="sxs-lookup"><span data-stu-id="c14e8-109">Type</span></span>   |<span data-ttu-id="c14e8-110">説明</span><span class="sxs-lookup"><span data-stu-id="c14e8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c14e8-111">policyType</span><span class="sxs-lookup"><span data-stu-id="c14e8-111">policyType</span></span>|<span data-ttu-id="c14e8-112">String</span><span class="sxs-lookup"><span data-stu-id="c14e8-112">String</span></span>|<span data-ttu-id="c14e8-113">ポリシーの名前を変更したり、変更の対象にされたことを示します</span><span class="sxs-lookup"><span data-stu-id="c14e8-113">Indicates the Policy Name that changed or was targetted for change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c14e8-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c14e8-114">JSON representation</span></span>

<span data-ttu-id="c14e8-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c14e8-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourcePolicy"
}-->

```json
{
  "policyType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourcePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
