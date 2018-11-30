---
title: targetResourceServicePrincipal リソースの種類
description: 監査活動、影響を受けるリソースの ServicePrincipalId を示します。 TargetResource リソースから派生します。
ms.openlocfilehash: 6d6e19997f4bfead771fc0230207df62dde6c6cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072398"
---
# <a name="targetresourceserviceprincipal-resource-type"></a><span data-ttu-id="10c8b-104">targetResourceServicePrincipal リソースの種類</span><span class="sxs-lookup"><span data-stu-id="10c8b-104">targetResourceServicePrincipal resource type</span></span>
<span data-ttu-id="10c8b-105">監査活動、影響を受けるリソースの ServicePrincipalId を示します。</span><span class="sxs-lookup"><span data-stu-id="10c8b-105">Indicates the ServicePrincipalId for the resource that impacted the audit activity.</span></span> <span data-ttu-id="10c8b-106">[TargetResource](targetresource.md)リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="10c8b-106">Derived from the [targetResource](targetresource.md) resource.</span></span>



## <a name="properties"></a><span data-ttu-id="10c8b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10c8b-107">Properties</span></span>
| <span data-ttu-id="10c8b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10c8b-108">Property</span></span>     | <span data-ttu-id="10c8b-109">型</span><span class="sxs-lookup"><span data-stu-id="10c8b-109">Type</span></span>   |<span data-ttu-id="10c8b-110">説明</span><span class="sxs-lookup"><span data-stu-id="10c8b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10c8b-111">appId</span><span class="sxs-lookup"><span data-stu-id="10c8b-111">appId</span></span>|<span data-ttu-id="10c8b-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="10c8b-112">String</span></span>|<span data-ttu-id="10c8b-113">アプリケーションの一意の Id を示します。</span><span class="sxs-lookup"><span data-stu-id="10c8b-113">Indicates the Unique Id of the application.</span></span> <span data-ttu-id="10c8b-114">固有のアプリケーションのアプリケーション Id を参照します。</span><span class="sxs-lookup"><span data-stu-id="10c8b-114">Refers to App Id for a specfic app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10c8b-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10c8b-115">JSON representation</span></span>

<span data-ttu-id="10c8b-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="10c8b-116">Here is a JSON representation of the resource.</span></span>

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