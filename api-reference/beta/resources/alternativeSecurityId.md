---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。 今後、この複合型は廃止されます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 32930b1e6dc5c4f58232d307dd67780d9b3981e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974333"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="d5d83-104">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5d83-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="d5d83-105">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="d5d83-105">For internal use only.</span></span> <span data-ttu-id="d5d83-106">今後、この複合型は廃止されます。</span><span class="sxs-lookup"><span data-stu-id="d5d83-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5d83-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5d83-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d5d83-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5d83-108">Properties</span></span>
| <span data-ttu-id="d5d83-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5d83-109">Property</span></span>         | <span data-ttu-id="d5d83-110">型</span><span class="sxs-lookup"><span data-stu-id="d5d83-110">Type</span></span>       | <span data-ttu-id="d5d83-111">説明</span><span class="sxs-lookup"><span data-stu-id="d5d83-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="d5d83-112">type</span><span class="sxs-lookup"><span data-stu-id="d5d83-112">type</span></span>             | <span data-ttu-id="d5d83-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d5d83-113">Int32</span></span>      | <span data-ttu-id="d5d83-114">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="d5d83-114">For internal use only</span></span>
| <span data-ttu-id="d5d83-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="d5d83-115">identityProvider</span></span> | <span data-ttu-id="d5d83-116">string</span><span class="sxs-lookup"><span data-stu-id="d5d83-116">string</span></span>     | <span data-ttu-id="d5d83-117">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="d5d83-117">For internal use only</span></span>
| <span data-ttu-id="d5d83-118">キー</span><span class="sxs-lookup"><span data-stu-id="d5d83-118">key</span></span>              | <span data-ttu-id="d5d83-119">Edm。バイナリ</span><span class="sxs-lookup"><span data-stu-id="d5d83-119">Edm.Binary</span></span> | <span data-ttu-id="d5d83-120">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="d5d83-120">For internal use only</span></span>
