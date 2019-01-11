---
title: targetResourceServicePrincipal リソースの種類
description: 監査活動、影響を受けるリソースの ServicePrincipalId を示します。 TargetResource リソースから派生します。
localization_priority: Normal
ms.openlocfilehash: 37bd63851ca9169afb669c710ef4cb2c150ea615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839600"
---
# <a name="targetresourceserviceprincipal-resource-type"></a><span data-ttu-id="3e022-104">targetResourceServicePrincipal リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e022-104">targetResourceServicePrincipal resource type</span></span>
<span data-ttu-id="3e022-105">監査活動、影響を受けるリソースの ServicePrincipalId を示します。</span><span class="sxs-lookup"><span data-stu-id="3e022-105">Indicates the ServicePrincipalId for the resource that impacted the audit activity.</span></span> <span data-ttu-id="3e022-106">[TargetResource](targetresource.md)リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="3e022-106">Derived from the [targetResource](targetresource.md) resource.</span></span>



## <a name="properties"></a><span data-ttu-id="3e022-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e022-107">Properties</span></span>
| <span data-ttu-id="3e022-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e022-108">Property</span></span>     | <span data-ttu-id="3e022-109">種類</span><span class="sxs-lookup"><span data-stu-id="3e022-109">Type</span></span>   |<span data-ttu-id="3e022-110">説明</span><span class="sxs-lookup"><span data-stu-id="3e022-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e022-111">appId</span><span class="sxs-lookup"><span data-stu-id="3e022-111">appId</span></span>|<span data-ttu-id="3e022-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3e022-112">String</span></span>|<span data-ttu-id="3e022-113">アプリケーションの一意の Id を示します。</span><span class="sxs-lookup"><span data-stu-id="3e022-113">Indicates the Unique Id of the application.</span></span> <span data-ttu-id="3e022-114">固有のアプリケーションのアプリケーション Id を参照します。</span><span class="sxs-lookup"><span data-stu-id="3e022-114">Refers to App Id for a specfic app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e022-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e022-115">JSON representation</span></span>

<span data-ttu-id="3e022-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3e022-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
