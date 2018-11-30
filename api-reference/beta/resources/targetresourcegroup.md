---
title: targetResourceGroup リソースの種類
description: '監査活動により影響を受けたグループの種類を示します。 Azure AD と統合されたグループと同じように値が含まれています '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069756"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="4fb74-104">targetResourceGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fb74-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="4fb74-105">監査活動により影響を受けたグループの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="4fb74-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="4fb74-106">Azure AD と統合されたグループと同じように値が含まれています</span><span class="sxs-lookup"><span data-stu-id="4fb74-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="4fb74-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb74-107">Properties</span></span>
| <span data-ttu-id="4fb74-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb74-108">Property</span></span>     | <span data-ttu-id="4fb74-109">型</span><span class="sxs-lookup"><span data-stu-id="4fb74-109">Type</span></span>   |<span data-ttu-id="4fb74-110">説明</span><span class="sxs-lookup"><span data-stu-id="4fb74-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fb74-111">groupType</span><span class="sxs-lookup"><span data-stu-id="4fb74-111">groupType</span></span>|<span data-ttu-id="4fb74-112">String</span><span class="sxs-lookup"><span data-stu-id="4fb74-112">String</span></span>| <span data-ttu-id="4fb74-113">可能な値は、`unifiedGroups`、`azureAD`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="4fb74-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4fb74-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fb74-114">JSON representation</span></span>

<span data-ttu-id="4fb74-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4fb74-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->