---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。 今後、この複合型は廃止されます。
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/20/2019
ms.locfileid: "35083943"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="0d27d-104">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d27d-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="0d27d-105">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="0d27d-105">For internal use only.</span></span> <span data-ttu-id="0d27d-106">今後、この複合型は廃止されます。</span><span class="sxs-lookup"><span data-stu-id="0d27d-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d27d-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d27d-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0d27d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d27d-108">Properties</span></span>
| <span data-ttu-id="0d27d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d27d-109">Property</span></span>         | <span data-ttu-id="0d27d-110">型</span><span class="sxs-lookup"><span data-stu-id="0d27d-110">Type</span></span>       | <span data-ttu-id="0d27d-111">説明</span><span class="sxs-lookup"><span data-stu-id="0d27d-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="0d27d-112">type</span><span class="sxs-lookup"><span data-stu-id="0d27d-112">type</span></span>             | <span data-ttu-id="0d27d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0d27d-113">Int32</span></span>      | <span data-ttu-id="0d27d-114">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="0d27d-114">For internal use only</span></span>
| <span data-ttu-id="0d27d-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="0d27d-115">identityProvider</span></span> | <span data-ttu-id="0d27d-116">string</span><span class="sxs-lookup"><span data-stu-id="0d27d-116">string</span></span>     | <span data-ttu-id="0d27d-117">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="0d27d-117">For internal use only</span></span>
| <span data-ttu-id="0d27d-118">キー</span><span class="sxs-lookup"><span data-stu-id="0d27d-118">key</span></span>              | <span data-ttu-id="0d27d-119">Edm。バイナリ</span><span class="sxs-lookup"><span data-stu-id="0d27d-119">Edm.Binary</span></span> | <span data-ttu-id="0d27d-120">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="0d27d-120">For internal use only</span></span>
