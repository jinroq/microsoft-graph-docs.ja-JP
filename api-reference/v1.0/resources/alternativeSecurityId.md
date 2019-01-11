---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853803"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="e55c0-103">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e55c0-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="e55c0-104">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="e55c0-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e55c0-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e55c0-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e55c0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e55c0-106">Properties</span></span>
| <span data-ttu-id="e55c0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e55c0-107">Property</span></span>         | <span data-ttu-id="e55c0-108">種類</span><span class="sxs-lookup"><span data-stu-id="e55c0-108">Type</span></span>       | <span data-ttu-id="e55c0-109">説明</span><span class="sxs-lookup"><span data-stu-id="e55c0-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="e55c0-110">type</span><span class="sxs-lookup"><span data-stu-id="e55c0-110">type</span></span>             | <span data-ttu-id="e55c0-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e55c0-111">Int32</span></span>      | <span data-ttu-id="e55c0-112">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="e55c0-112">For internal use only</span></span>
| <span data-ttu-id="e55c0-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="e55c0-113">identityProvider</span></span> | <span data-ttu-id="e55c0-114">文字列</span><span class="sxs-lookup"><span data-stu-id="e55c0-114">string</span></span>     | <span data-ttu-id="e55c0-115">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="e55c0-115">For internal use only</span></span>
| <span data-ttu-id="e55c0-116">Key</span><span class="sxs-lookup"><span data-stu-id="e55c0-116">key</span></span>              | <span data-ttu-id="e55c0-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="e55c0-117">Edm.Binary</span></span> | <span data-ttu-id="e55c0-118">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="e55c0-118">For internal use only</span></span>
