---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
ms.openlocfilehash: 9d941469da133d9a3e7149dfca55c813f60b3ce8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020227"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="93124-103">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93124-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="93124-104">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="93124-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93124-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93124-105">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a><span data-ttu-id="93124-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93124-106">Properties</span></span>
| <span data-ttu-id="93124-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93124-107">Property</span></span>         | <span data-ttu-id="93124-108">型</span><span class="sxs-lookup"><span data-stu-id="93124-108">Type</span></span>       | <span data-ttu-id="93124-109">説明</span><span class="sxs-lookup"><span data-stu-id="93124-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="93124-110">type</span><span class="sxs-lookup"><span data-stu-id="93124-110">type</span></span>             | <span data-ttu-id="93124-111">Int32</span><span class="sxs-lookup"><span data-stu-id="93124-111">Int32</span></span>      | <span data-ttu-id="93124-112">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="93124-112">For internal use only</span></span>
| <span data-ttu-id="93124-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="93124-113">identityProvider</span></span> | <span data-ttu-id="93124-114">文字列</span><span class="sxs-lookup"><span data-stu-id="93124-114">string</span></span>     | <span data-ttu-id="93124-115">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="93124-115">For internal use only</span></span>
| <span data-ttu-id="93124-116">Key</span><span class="sxs-lookup"><span data-stu-id="93124-116">key</span></span>              | <span data-ttu-id="93124-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="93124-117">Edm.Binary</span></span> | <span data-ttu-id="93124-118">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="93124-118">For internal use only</span></span>
