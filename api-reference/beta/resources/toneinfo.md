---
title: toneInfo リソースの種類
description: 1つの DTMF イベント。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0eaa4b4159ffd5e7455b1155a7f3cd82c89b19aa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964250"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="4b297-103">toneInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b297-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b297-104">1つの DTMF イベント。</span><span class="sxs-lookup"><span data-stu-id="4b297-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="4b297-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b297-105">Properties</span></span>

| <span data-ttu-id="4b297-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b297-106">Property</span></span>       | <span data-ttu-id="4b297-107">型</span><span class="sxs-lookup"><span data-stu-id="4b297-107">Type</span></span>    | <span data-ttu-id="4b297-108">説明</span><span class="sxs-lookup"><span data-stu-id="4b297-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b297-109">sequenceId</span><span class="sxs-lookup"><span data-stu-id="4b297-109">sequenceId</span></span> | <span data-ttu-id="4b297-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4b297-110">Int64</span></span> | <span data-ttu-id="4b297-111">DTMF イベントの順序付けに使用される増分識別子。</span><span class="sxs-lookup"><span data-stu-id="4b297-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="4b297-112">低音</span><span class="sxs-lookup"><span data-stu-id="4b297-112">tone</span></span> | <span data-ttu-id="4b297-113">String</span><span class="sxs-lookup"><span data-stu-id="4b297-113">String</span></span> | <span data-ttu-id="4b297-114">可能な値は`tone0`、 `tone1`、 `tone2` `tone3` `tone4` `tone5` `tone6` `tone7` `tone8` `flash`、、 `star`、、、、、、、、です。 `tone9` `pound` `a` `b` `c` `d`</span><span class="sxs-lookup"><span data-stu-id="4b297-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4b297-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b297-115">JSON representation</span></span>

<span data-ttu-id="4b297-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b297-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
