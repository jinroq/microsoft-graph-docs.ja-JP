---
title: callroute リソースの種類
description: callroute の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06dd1a2265c5a6bda9feba0b51e7fd731d7945c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328278"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="e9dd5-103">callroute リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9dd5-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9dd5-104">callroute の種類。</span><span class="sxs-lookup"><span data-stu-id="e9dd5-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="e9dd5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9dd5-105">Properties</span></span>

| <span data-ttu-id="e9dd5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9dd5-106">Property</span></span>            | <span data-ttu-id="e9dd5-107">型</span><span class="sxs-lookup"><span data-stu-id="e9dd5-107">Type</span></span>                          | <span data-ttu-id="e9dd5-108">説明</span><span class="sxs-lookup"><span data-stu-id="e9dd5-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="e9dd5-109">最終的な</span><span class="sxs-lookup"><span data-stu-id="e9dd5-109">final</span></span>               | [<span data-ttu-id="e9dd5-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9dd5-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="e9dd5-111">呼び出しで解決された id。</span><span class="sxs-lookup"><span data-stu-id="e9dd5-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="e9dd5-112">翻訳元</span><span class="sxs-lookup"><span data-stu-id="e9dd5-112">original</span></span>            | [<span data-ttu-id="e9dd5-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9dd5-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="e9dd5-114">最初に呼び出しで使用された id。</span><span class="sxs-lookup"><span data-stu-id="e9dd5-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="e9dd5-115">routingtype</span><span class="sxs-lookup"><span data-stu-id="e9dd5-115">routingType</span></span>         | <span data-ttu-id="e9dd5-116">String</span><span class="sxs-lookup"><span data-stu-id="e9dd5-116">String</span></span>                        | <span data-ttu-id="e9dd5-117">可能な値は、`forwarded`、`lookup`、`selfFork` です。</span><span class="sxs-lookup"><span data-stu-id="e9dd5-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e9dd5-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9dd5-118">JSON representation</span></span>

<span data-ttu-id="e9dd5-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9dd5-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
