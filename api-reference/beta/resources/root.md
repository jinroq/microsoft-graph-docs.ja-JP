---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 原因
localization_priority: Normal
ms.openlocfilehash: 83211263f4ba7998ea9e1863756f5aba7b6ff070
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343508"
---
# <a name="root-resource-type"></a><span data-ttu-id="37f38-102">Root リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37f38-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37f38-103">**Root** ファセットは、オブジェクトが階層内の最上位であることを示します。</span><span class="sxs-lookup"><span data-stu-id="37f38-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="37f38-104">このファセットに値が存在する (null ではない) ことで、オブジェクトがルートであることを示します。</span><span class="sxs-lookup"><span data-stu-id="37f38-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="37f38-105">null (または存在しない) 値は、オブジェクトがルートでないことを示します。</span><span class="sxs-lookup"><span data-stu-id="37f38-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="37f38-106">**注**:現在、このファセットは空ですが、将来のリビジョンでは、このファセットに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="37f38-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37f38-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37f38-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="37f38-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37f38-108">Properties</span></span>

<span data-ttu-id="37f38-109">**ルート** リソースにはプロパティがありません。</span><span class="sxs-lookup"><span data-stu-id="37f38-109">The **Root** resource has no properties.</span></span>


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": []
}
-->
