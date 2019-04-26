---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: incompletedata
localization_priority: Normal
ms.openlocfilehash: 40c1b782384076eefc986f67dc1736f191feb7b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339967"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="720eb-102">incompletedata リソースの種類</span><span class="sxs-lookup"><span data-stu-id="720eb-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="720eb-103">**incompletedata**ファセットは、リソースが不完全なデータで生成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="720eb-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="720eb-104">内のプロパティは、データが不完全である理由についての情報を提供する場合があります。</span><span class="sxs-lookup"><span data-stu-id="720eb-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="720eb-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="720eb-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="720eb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="720eb-106">Properties</span></span>

| <span data-ttu-id="720eb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="720eb-107">Property</span></span>                  | <span data-ttu-id="720eb-108">型</span><span class="sxs-lookup"><span data-stu-id="720eb-108">Type</span></span>           | <span data-ttu-id="720eb-109">説明</span><span class="sxs-lookup"><span data-stu-id="720eb-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="720eb-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="720eb-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="720eb-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="720eb-111">DateTimeOffset</span></span> | <span data-ttu-id="720eb-112">サービスは、指定された時間の前にソースデータを持っていません。</span><span class="sxs-lookup"><span data-stu-id="720eb-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="720eb-113">制限あり</span><span class="sxs-lookup"><span data-stu-id="720eb-113">wasThrottled</span></span>              | <span data-ttu-id="720eb-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="720eb-114">Boolean</span></span>        | <span data-ttu-id="720eb-115">アクティビティが多すぎるため、一部のデータが記録されませんでした。</span><span class="sxs-lookup"><span data-stu-id="720eb-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
