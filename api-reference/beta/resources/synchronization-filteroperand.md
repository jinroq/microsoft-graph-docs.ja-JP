---
title: filterOperand リソースの種類
description: オペランドの値のコレクションが含まれています。
ms.openlocfilehash: 8fa4d12efd9fc2b5afa7f250d2ed3f98ed092d06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073169"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="dc170-103">filterOperand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc170-103">filterOperand resource type</span></span>

> <span data-ttu-id="dc170-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc170-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc170-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc170-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc170-106">オペランドの値のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dc170-106">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="dc170-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc170-107">Properties</span></span>
| <span data-ttu-id="dc170-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc170-108">Property</span></span>     | <span data-ttu-id="dc170-109">型</span><span class="sxs-lookup"><span data-stu-id="dc170-109">Type</span></span>   |<span data-ttu-id="dc170-110">説明</span><span class="sxs-lookup"><span data-stu-id="dc170-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc170-111">values</span><span class="sxs-lookup"><span data-stu-id="dc170-111">values</span></span>|<span data-ttu-id="dc170-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dc170-112">String collection</span></span>|<span data-ttu-id="dc170-113">値のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="dc170-113">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc170-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc170-114">JSON representation</span></span>

<span data-ttu-id="dc170-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc170-115">The following is a JSON representation of the resource.</span></span>

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