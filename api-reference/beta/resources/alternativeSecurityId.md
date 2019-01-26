---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
ms.openlocfilehash: 9d941469da133d9a3e7149dfca55c813f60b3ce8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29579843"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="03bf8-103">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03bf8-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="03bf8-104">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="03bf8-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03bf8-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03bf8-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="03bf8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03bf8-106">Properties</span></span>
| <span data-ttu-id="03bf8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03bf8-107">Property</span></span>         | <span data-ttu-id="03bf8-108">型</span><span class="sxs-lookup"><span data-stu-id="03bf8-108">Type</span></span>       | <span data-ttu-id="03bf8-109">説明</span><span class="sxs-lookup"><span data-stu-id="03bf8-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="03bf8-110">type</span><span class="sxs-lookup"><span data-stu-id="03bf8-110">type</span></span>             | <span data-ttu-id="03bf8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="03bf8-111">Int32</span></span>      | <span data-ttu-id="03bf8-112">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="03bf8-112">For internal use only</span></span>
| <span data-ttu-id="03bf8-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="03bf8-113">identityProvider</span></span> | <span data-ttu-id="03bf8-114">文字列</span><span class="sxs-lookup"><span data-stu-id="03bf8-114">string</span></span>     | <span data-ttu-id="03bf8-115">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="03bf8-115">For internal use only</span></span>
| <span data-ttu-id="03bf8-116">Key</span><span class="sxs-lookup"><span data-stu-id="03bf8-116">key</span></span>              | <span data-ttu-id="03bf8-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="03bf8-117">Edm.Binary</span></span> | <span data-ttu-id="03bf8-118">内部使用のみ。 </span><span class="sxs-lookup"><span data-stu-id="03bf8-118">For internal use only</span></span>
