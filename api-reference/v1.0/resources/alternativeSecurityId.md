---
title: alternativeSecurityId リソースの種類
description: 内部使用のみ。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d4cdfa609e5cc2daf484bf0f35b863285ee811dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033244"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="b1983-103">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1983-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="b1983-104">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="b1983-104">For internal use only.</span></span> <span data-ttu-id="b1983-105">今後、この複合型は廃止されます。</span><span class="sxs-lookup"><span data-stu-id="b1983-105">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1983-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1983-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b1983-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1983-107">Properties</span></span>
| <span data-ttu-id="b1983-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1983-108">Property</span></span>         | <span data-ttu-id="b1983-109">型</span><span class="sxs-lookup"><span data-stu-id="b1983-109">Type</span></span>       | <span data-ttu-id="b1983-110">説明</span><span class="sxs-lookup"><span data-stu-id="b1983-110">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="b1983-111">type</span><span class="sxs-lookup"><span data-stu-id="b1983-111">type</span></span>             | <span data-ttu-id="b1983-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b1983-112">Int32</span></span>      | <span data-ttu-id="b1983-113">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="b1983-113">For internal use only</span></span>
| <span data-ttu-id="b1983-114">identityProvider</span><span class="sxs-lookup"><span data-stu-id="b1983-114">identityProvider</span></span> | <span data-ttu-id="b1983-115">string</span><span class="sxs-lookup"><span data-stu-id="b1983-115">string</span></span>     | <span data-ttu-id="b1983-116">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="b1983-116">For internal use only</span></span>
| <span data-ttu-id="b1983-117">キー</span><span class="sxs-lookup"><span data-stu-id="b1983-117">key</span></span>              | <span data-ttu-id="b1983-118">Edm。バイナリ</span><span class="sxs-lookup"><span data-stu-id="b1983-118">Edm.Binary</span></span> | <span data-ttu-id="b1983-119">システム内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="b1983-119">For internal use only</span></span>
