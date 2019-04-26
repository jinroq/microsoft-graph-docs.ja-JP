---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
localization_priority: Normal
ms.openlocfilehash: 60e45c6d914c64f92b9f15f78fda22372a23e91f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345842"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="47fd6-103">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47fd6-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="47fd6-104">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="47fd6-104">For internal use only.</span></span> <span data-ttu-id="47fd6-105">今後、この複合型は廃止されます。</span><span class="sxs-lookup"><span data-stu-id="47fd6-105">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47fd6-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47fd6-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="47fd6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47fd6-107">Properties</span></span>
| <span data-ttu-id="47fd6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47fd6-108">Property</span></span>         | <span data-ttu-id="47fd6-109">型</span><span class="sxs-lookup"><span data-stu-id="47fd6-109">Type</span></span>       | <span data-ttu-id="47fd6-110">説明</span><span class="sxs-lookup"><span data-stu-id="47fd6-110">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="47fd6-111">type</span><span class="sxs-lookup"><span data-stu-id="47fd6-111">type</span></span>             | <span data-ttu-id="47fd6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="47fd6-112">Int32</span></span>      | <span data-ttu-id="47fd6-113">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="47fd6-113">For internal use only</span></span>
| <span data-ttu-id="47fd6-114">identityProvider</span><span class="sxs-lookup"><span data-stu-id="47fd6-114">identityProvider</span></span> | <span data-ttu-id="47fd6-115">string</span><span class="sxs-lookup"><span data-stu-id="47fd6-115">string</span></span>     | <span data-ttu-id="47fd6-116">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="47fd6-116">For internal use only</span></span>
| <span data-ttu-id="47fd6-117">キー</span><span class="sxs-lookup"><span data-stu-id="47fd6-117">key</span></span>              | <span data-ttu-id="47fd6-118">Edm。バイナリ</span><span class="sxs-lookup"><span data-stu-id="47fd6-118">Edm.Binary</span></span> | <span data-ttu-id="47fd6-119">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="47fd6-119">For internal use only</span></span>
