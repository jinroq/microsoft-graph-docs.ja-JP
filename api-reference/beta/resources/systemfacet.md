---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: SystemFacet
localization_priority: Normal
ms.openlocfilehash: afafb69e9d887d2cb8d9537dd7ef9d3a712f3333
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528551"
---
# <a name="system-facet"></a><span data-ttu-id="48554-102">System ファセット</span><span class="sxs-lookup"><span data-stu-id="48554-102">System facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48554-103">**System** ファセットは、オブジェクトが自身の操作のためにシステムによって管理されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="48554-103">The **System** facet indicates that the object is managed by the system for its own operation.</span></span>
<span data-ttu-id="48554-104">アプリの多くは System ファセットを持つアイテムを無視すべきです。</span><span class="sxs-lookup"><span data-stu-id="48554-104">Most apps should ignore items that have a System facet.</span></span>

<span data-ttu-id="48554-105">**注**:現在、このファセットは空ですが、将来のリビジョンでは、このファセットに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="48554-105">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="48554-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48554-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.systemFacet", "@type.aka": "microsoft.graph.systemFacet" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="48554-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48554-107">Properties</span></span>

<span data-ttu-id="48554-108">なし。</span><span class="sxs-lookup"><span data-stu-id="48554-108">None.</span></span> <span data-ttu-id="48554-109">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="48554-109">This facet is a null or not-null value and contains no properties.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/System",
  "suppressions": [
    "Error: /api-reference/beta/resources/systemfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
