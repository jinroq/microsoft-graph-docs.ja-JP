---
author: daspek
description: IncompleteData ファセットは、リソースが不完全なデータで生成されたことを示します。
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 23d78fa3605259031fc2c408e93a0461bb12cb28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006284"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="4fb91-103">incompleteData リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fb91-103">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fb91-104">**Incompletedata**ファセットは、リソースが不完全なデータで生成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb91-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="4fb91-105">内のプロパティは、データが不完全である理由についての情報を提供する場合があります。</span><span class="sxs-lookup"><span data-stu-id="4fb91-105">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fb91-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fb91-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="4fb91-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb91-107">Properties</span></span>

| <span data-ttu-id="4fb91-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb91-108">Property</span></span>                  | <span data-ttu-id="4fb91-109">型</span><span class="sxs-lookup"><span data-stu-id="4fb91-109">Type</span></span>           | <span data-ttu-id="4fb91-110">説明</span><span class="sxs-lookup"><span data-stu-id="4fb91-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="4fb91-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="4fb91-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="4fb91-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fb91-112">DateTimeOffset</span></span> | <span data-ttu-id="4fb91-113">サービスは、指定された時間の前にソースデータを持っていません。</span><span class="sxs-lookup"><span data-stu-id="4fb91-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="4fb91-114">制限あり</span><span class="sxs-lookup"><span data-stu-id="4fb91-114">wasThrottled</span></span>              | <span data-ttu-id="4fb91-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb91-115">Boolean</span></span>        | <span data-ttu-id="4fb91-116">アクティビティが多すぎるため、一部のデータが記録されませんでした。</span><span class="sxs-lookup"><span data-stu-id="4fb91-116">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
