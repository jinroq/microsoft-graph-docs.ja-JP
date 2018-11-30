---
title: targetResourcePolicy リソースの種類
description: '監査活動によって影響を与えたのポリシーを示します。 TargetResource リソースから派生します。   '
ms.openlocfilehash: 20486c535d0df4b3745f5cfc3414b320a9374075
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071756"
---
# <a name="targetresourcepolicy-resource-type"></a><span data-ttu-id="73491-104">targetResourcePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73491-104">targetResourcePolicy resource type</span></span>
<span data-ttu-id="73491-105">監査活動によって影響を与えたのポリシーを示します。</span><span class="sxs-lookup"><span data-stu-id="73491-105">Indicates the policy that was impacted by the audit activity.</span></span> <span data-ttu-id="73491-106">[TargetResource](targetresource.md)リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="73491-106">Derived from the [targetResource](targetresource.md) resource.</span></span>   



## <a name="properties"></a><span data-ttu-id="73491-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73491-107">Properties</span></span>
| <span data-ttu-id="73491-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73491-108">Property</span></span>     | <span data-ttu-id="73491-109">型</span><span class="sxs-lookup"><span data-stu-id="73491-109">Type</span></span>   |<span data-ttu-id="73491-110">説明</span><span class="sxs-lookup"><span data-stu-id="73491-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73491-111">policyType</span><span class="sxs-lookup"><span data-stu-id="73491-111">policyType</span></span>|<span data-ttu-id="73491-112">String</span><span class="sxs-lookup"><span data-stu-id="73491-112">String</span></span>|<span data-ttu-id="73491-113">ポリシーの名前を変更したり、変更の対象にされたことを示します</span><span class="sxs-lookup"><span data-stu-id="73491-113">Indicates the Policy Name that changed or was targetted for change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73491-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73491-114">JSON representation</span></span>

<span data-ttu-id="73491-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="73491-115">Here is a JSON representation of the resource.</span></span>

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