---
title: FilterCriteria リソースの種類
description: 列に適用するフィルター条件を表します。
ms.openlocfilehash: dbcc57ff940fec525b712eb11ac44209f5f8a4d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067172"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="f125d-103">FilterCriteria リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f125d-103">FilterCriteria resource type</span></span>

> <span data-ttu-id="f125d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f125d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f125d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f125d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f125d-106">列に適用するフィルター条件を表します。</span><span class="sxs-lookup"><span data-stu-id="f125d-106">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f125d-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f125d-107">JSON representation</span></span>

<span data-ttu-id="f125d-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f125d-108">Here is a JSON representation of the resource.</span></span>

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