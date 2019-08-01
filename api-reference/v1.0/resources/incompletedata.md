---
author: daspek
ms.author: dspektor
title: incompleteData リソースの種類
description: IncompleteData ファセットは、リソースが不完全なデータで生成されたことを示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0ac77c5dc4daed9330c4fb71185e9505feee5048
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029240"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="7ec5a-103">incompleteData リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7ec5a-103">incompleteData resource type</span></span>

<span data-ttu-id="7ec5a-104">**Incompletedata**ファセットは、リソースが不完全なデータで生成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="7ec5a-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="7ec5a-105">内のプロパティは、データが不完全である理由についての情報を提供する場合があります。</span><span class="sxs-lookup"><span data-stu-id="7ec5a-105">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="7ec5a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ec5a-106">Properties</span></span>

| <span data-ttu-id="7ec5a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ec5a-107">Property</span></span>                  | <span data-ttu-id="7ec5a-108">型</span><span class="sxs-lookup"><span data-stu-id="7ec5a-108">Type</span></span>           | <span data-ttu-id="7ec5a-109">説明</span><span class="sxs-lookup"><span data-stu-id="7ec5a-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="7ec5a-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="7ec5a-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="7ec5a-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ec5a-111">DateTimeOffset</span></span> | <span data-ttu-id="7ec5a-112">サービスは、指定された時間の前にソースデータを持っていません。</span><span class="sxs-lookup"><span data-stu-id="7ec5a-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="7ec5a-113">制限あり</span><span class="sxs-lookup"><span data-stu-id="7ec5a-113">wasThrottled</span></span>              | <span data-ttu-id="7ec5a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ec5a-114">Boolean</span></span>        | <span data-ttu-id="7ec5a-115">アクティビティが多すぎるため、一部のデータが記録されませんでした。</span><span class="sxs-lookup"><span data-stu-id="7ec5a-115">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ec5a-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ec5a-116">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->
