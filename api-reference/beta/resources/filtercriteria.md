---
title: FilterCriteria リソースの種類
description: 列に適用するフィルター条件を表します。
localization_priority: Normal
ms.openlocfilehash: 56663e802aacc2dab3f08462724d0994b5bada85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821680"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="e8d1a-103">FilterCriteria リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8d1a-103">FilterCriteria resource type</span></span>

> <span data-ttu-id="e8d1a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8d1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8d1a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8d1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8d1a-106">列に適用するフィルター条件を表します。</span><span class="sxs-lookup"><span data-stu-id="e8d1a-106">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8d1a-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8d1a-107">JSON representation</span></span>

<span data-ttu-id="e8d1a-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8d1a-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": "string"
}

```
