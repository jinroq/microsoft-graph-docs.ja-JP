---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525088"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="ce1f6-102">incompleteData リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce1f6-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce1f6-103">**IncompleteData**ファセットは、不完全なデータとリソースが生成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="ce1f6-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="ce1f6-104">内でプロパティがについての情報を提供するには、不完全なデータがある理由です。</span><span class="sxs-lookup"><span data-stu-id="ce1f6-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce1f6-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce1f6-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="ce1f6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce1f6-106">Properties</span></span>

| <span data-ttu-id="ce1f6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce1f6-107">Property</span></span>                  | <span data-ttu-id="ce1f6-108">型</span><span class="sxs-lookup"><span data-stu-id="ce1f6-108">Type</span></span>           | <span data-ttu-id="ce1f6-109">説明</span><span class="sxs-lookup"><span data-stu-id="ce1f6-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="ce1f6-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="ce1f6-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="ce1f6-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce1f6-111">DateTimeOffset</span></span> | <span data-ttu-id="ce1f6-112">サービスには、指定された時間の前にソース データがありません。</span><span class="sxs-lookup"><span data-stu-id="ce1f6-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="ce1f6-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="ce1f6-113">wasThrottled</span></span>              | <span data-ttu-id="ce1f6-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="ce1f6-114">Boolean</span></span>        | <span data-ttu-id="ce1f6-115">データの一部は、過剰な活動のため録画されませんでした。</span><span class="sxs-lookup"><span data-stu-id="ce1f6-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": [
    "Error: /api-reference/beta/resources/incompletedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
