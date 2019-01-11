---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: add1e3612f65e203f2437419cbb105b78025aa0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807512"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="77cc6-102">incompleteData リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77cc6-102">incompleteData resource type</span></span>

 > <span data-ttu-id="77cc6-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77cc6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77cc6-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77cc6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77cc6-105">**IncompleteData**ファセットは、不完全なデータとリソースが生成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="77cc6-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="77cc6-106">内でプロパティがについての情報を提供するには、不完全なデータがある理由です。</span><span class="sxs-lookup"><span data-stu-id="77cc6-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77cc6-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77cc6-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="77cc6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77cc6-108">Properties</span></span>

| <span data-ttu-id="77cc6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77cc6-109">Property</span></span>                  | <span data-ttu-id="77cc6-110">種類</span><span class="sxs-lookup"><span data-stu-id="77cc6-110">Type</span></span>           | <span data-ttu-id="77cc6-111">説明</span><span class="sxs-lookup"><span data-stu-id="77cc6-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="77cc6-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="77cc6-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="77cc6-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77cc6-113">DateTimeOffset</span></span> | <span data-ttu-id="77cc6-114">サービスには、指定された時間の前にソース データがありません。</span><span class="sxs-lookup"><span data-stu-id="77cc6-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="77cc6-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="77cc6-115">wasThrottled</span></span>              | <span data-ttu-id="77cc6-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="77cc6-116">Boolean</span></span>        | <span data-ttu-id="77cc6-117">データの一部は、過剰な活動のため録画されませんでした。</span><span class="sxs-lookup"><span data-stu-id="77cc6-117">Some data was not recorded due to excessive activity.</span></span>

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
