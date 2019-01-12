---
title: toneInfo リソースの種類
description: 1 つの DTMF イベントです。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 479697ea847f3a943e1d9bb7de19c422d15b47c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916972"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="c3898-103">toneInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3898-103">toneInfo resource type</span></span>

> <span data-ttu-id="c3898-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3898-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3898-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3898-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3898-106">1 つの DTMF イベントです。</span><span class="sxs-lookup"><span data-stu-id="c3898-106">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="c3898-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3898-107">Properties</span></span>

| <span data-ttu-id="c3898-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3898-108">Property</span></span>       | <span data-ttu-id="c3898-109">種類</span><span class="sxs-lookup"><span data-stu-id="c3898-109">Type</span></span>    | <span data-ttu-id="c3898-110">説明</span><span class="sxs-lookup"><span data-stu-id="c3898-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3898-111">sequenceId</span><span class="sxs-lookup"><span data-stu-id="c3898-111">sequenceId</span></span> | <span data-ttu-id="c3898-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c3898-112">Int64</span></span> | <span data-ttu-id="c3898-113">DTMF イベントの順序付けに使用される増分の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c3898-113">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="c3898-114">トーン</span><span class="sxs-lookup"><span data-stu-id="c3898-114">tone</span></span> | <span data-ttu-id="c3898-115">String</span><span class="sxs-lookup"><span data-stu-id="c3898-115">String</span></span> | <span data-ttu-id="c3898-116">使用可能な値: `tone0`、 `tone1`、 `tone2`、 `tone3`、 `tone4`、 `tone5`、 `tone6`、 `tone7`、 `tone8`、 `tone9`、 `star`、 `pound`、 `a`、 `b`、 `c`、 `d`、 `flash`。</span><span class="sxs-lookup"><span data-stu-id="c3898-116">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3898-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3898-117">JSON representation</span></span>

<span data-ttu-id="c3898-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c3898-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
