---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: incompletedata
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549035"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="fe94c-102">incompletedata リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe94c-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe94c-103">**incompletedata**ファセットは、リソースが不完全なデータで生成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="fe94c-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="fe94c-104">内のプロパティは、データが不完全である理由についての情報を提供する場合があります。</span><span class="sxs-lookup"><span data-stu-id="fe94c-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe94c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe94c-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="fe94c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe94c-106">Properties</span></span>

| <span data-ttu-id="fe94c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe94c-107">Property</span></span>                  | <span data-ttu-id="fe94c-108">型</span><span class="sxs-lookup"><span data-stu-id="fe94c-108">Type</span></span>           | <span data-ttu-id="fe94c-109">説明</span><span class="sxs-lookup"><span data-stu-id="fe94c-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="fe94c-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="fe94c-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="fe94c-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe94c-111">DateTimeOffset</span></span> | <span data-ttu-id="fe94c-112">サービスは、指定された時間の前にソースデータを持っていません。</span><span class="sxs-lookup"><span data-stu-id="fe94c-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="fe94c-113">制限あり</span><span class="sxs-lookup"><span data-stu-id="fe94c-113">wasThrottled</span></span>              | <span data-ttu-id="fe94c-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="fe94c-114">Boolean</span></span>        | <span data-ttu-id="fe94c-115">アクティビティが多すぎるため、一部のデータが記録されませんでした。</span><span class="sxs-lookup"><span data-stu-id="fe94c-115">Some data was not recorded due to excessive activity.</span></span>

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
