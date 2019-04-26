---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569481"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="dc5cc-103">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc5cc-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="dc5cc-104">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc5cc-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc5cc-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="dc5cc-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc5cc-106">Properties</span></span>
| <span data-ttu-id="dc5cc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc5cc-107">Property</span></span>         | <span data-ttu-id="dc5cc-108">型</span><span class="sxs-lookup"><span data-stu-id="dc5cc-108">Type</span></span>       | <span data-ttu-id="dc5cc-109">説明</span><span class="sxs-lookup"><span data-stu-id="dc5cc-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="dc5cc-110">type</span><span class="sxs-lookup"><span data-stu-id="dc5cc-110">type</span></span>             | <span data-ttu-id="dc5cc-111">Int32</span><span class="sxs-lookup"><span data-stu-id="dc5cc-111">Int32</span></span>      | <span data-ttu-id="dc5cc-112">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-112">For internal use only</span></span>
| <span data-ttu-id="dc5cc-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="dc5cc-113">identityProvider</span></span> | <span data-ttu-id="dc5cc-114">string</span><span class="sxs-lookup"><span data-stu-id="dc5cc-114">string</span></span>     | <span data-ttu-id="dc5cc-115">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-115">For internal use only</span></span>
| <span data-ttu-id="dc5cc-116">キー</span><span class="sxs-lookup"><span data-stu-id="dc5cc-116">key</span></span>              | <span data-ttu-id="dc5cc-117">Edm。バイナリ</span><span class="sxs-lookup"><span data-stu-id="dc5cc-117">Edm.Binary</span></span> | <span data-ttu-id="dc5cc-118">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-118">For internal use only</span></span>
