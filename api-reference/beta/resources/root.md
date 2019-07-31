---
author: JeremyKelley
description: Root ファセットは、オブジェクトが階層内の最上位であることを示します。
ms.date: 09/10/2017
title: 原因
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 78a0bd7da9ab0d2f6f0c15a06416ce09ae53219a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008650"
---
# <a name="root-resource-type"></a><span data-ttu-id="cde85-103">Root リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cde85-103">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cde85-104">**Root** ファセットは、オブジェクトが階層内の最上位であることを示します。</span><span class="sxs-lookup"><span data-stu-id="cde85-104">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="cde85-105">このファセットに値が存在する (null ではない) ことで、オブジェクトがルートであることを示します。</span><span class="sxs-lookup"><span data-stu-id="cde85-105">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="cde85-106">null (または存在しない) 値は、オブジェクトがルートでないことを示します。</span><span class="sxs-lookup"><span data-stu-id="cde85-106">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="cde85-107">**注**:現在、このファセットは空ですが、将来のリビジョンでは、このファセットに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cde85-107">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cde85-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cde85-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="cde85-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cde85-109">Properties</span></span>

<span data-ttu-id="cde85-110">**ルート** リソースにはプロパティがありません。</span><span class="sxs-lookup"><span data-stu-id="cde85-110">The **Root** resource has no properties.</span></span>


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": []
}
-->
