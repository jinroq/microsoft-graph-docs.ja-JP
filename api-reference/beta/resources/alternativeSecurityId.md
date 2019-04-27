---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。 今後、この複合型は廃止されます。
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348402"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="fa9f7-104">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa9f7-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="fa9f7-105">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="fa9f7-105">For internal use only.</span></span> <span data-ttu-id="fa9f7-106">今後、この複合型は廃止されます。</span><span class="sxs-lookup"><span data-stu-id="fa9f7-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa9f7-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa9f7-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fa9f7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa9f7-108">Properties</span></span>
| <span data-ttu-id="fa9f7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa9f7-109">Property</span></span>         | <span data-ttu-id="fa9f7-110">種類</span><span class="sxs-lookup"><span data-stu-id="fa9f7-110">Type</span></span>       | <span data-ttu-id="fa9f7-111">説明</span><span class="sxs-lookup"><span data-stu-id="fa9f7-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="fa9f7-112">type</span><span class="sxs-lookup"><span data-stu-id="fa9f7-112">type</span></span>             | <span data-ttu-id="fa9f7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="fa9f7-113">Int32</span></span>      | <span data-ttu-id="fa9f7-114">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="fa9f7-114">For internal use only</span></span>
| <span data-ttu-id="fa9f7-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="fa9f7-115">identityProvider</span></span> | <span data-ttu-id="fa9f7-116">string</span><span class="sxs-lookup"><span data-stu-id="fa9f7-116">string</span></span>     | <span data-ttu-id="fa9f7-117">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="fa9f7-117">For internal use only</span></span>
| <span data-ttu-id="fa9f7-118">キー</span><span class="sxs-lookup"><span data-stu-id="fa9f7-118">key</span></span>              | <span data-ttu-id="fa9f7-119">Edm。バイナリ</span><span class="sxs-lookup"><span data-stu-id="fa9f7-119">Edm.Binary</span></span> | <span data-ttu-id="fa9f7-120">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="fa9f7-120">For internal use only</span></span>
