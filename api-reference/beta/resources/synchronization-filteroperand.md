---
title: filterOperand リソースの種類
description: オペランドの値のコレクションが含まれています。
localization_priority: Normal
ms.openlocfilehash: 5c2154eda43a95ce2c7e5966e43c0b6a1fafe68e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884421"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="a39a7-103">filterOperand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a39a7-103">filterOperand resource type</span></span>

> <span data-ttu-id="a39a7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a39a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a39a7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a39a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a39a7-106">オペランドの値のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a39a7-106">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="a39a7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a39a7-107">Properties</span></span>
| <span data-ttu-id="a39a7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a39a7-108">Property</span></span>     | <span data-ttu-id="a39a7-109">種類</span><span class="sxs-lookup"><span data-stu-id="a39a7-109">Type</span></span>   |<span data-ttu-id="a39a7-110">説明</span><span class="sxs-lookup"><span data-stu-id="a39a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a39a7-111">values</span><span class="sxs-lookup"><span data-stu-id="a39a7-111">values</span></span>|<span data-ttu-id="a39a7-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a39a7-112">String collection</span></span>|<span data-ttu-id="a39a7-113">値のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a39a7-113">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a39a7-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a39a7-114">JSON representation</span></span>

<span data-ttu-id="a39a7-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a39a7-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperand"
}-->

```json
{
  "values": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterOperand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
