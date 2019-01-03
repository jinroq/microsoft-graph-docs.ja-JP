---
title: toneInfo リソースの種類
description: 1 つの DTMF イベントです。
author: VinodRavichandran
ms.openlocfilehash: 0ae78a9a4721c88767ebc460a99c7cdea30f44c5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380339"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="0d888-103">toneInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d888-103">toneInfo resource type</span></span>

> <span data-ttu-id="0d888-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d888-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d888-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d888-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d888-106">1 つの DTMF イベントです。</span><span class="sxs-lookup"><span data-stu-id="0d888-106">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="0d888-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d888-107">Properties</span></span>

| <span data-ttu-id="0d888-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d888-108">Property</span></span>       | <span data-ttu-id="0d888-109">型</span><span class="sxs-lookup"><span data-stu-id="0d888-109">Type</span></span>    | <span data-ttu-id="0d888-110">説明</span><span class="sxs-lookup"><span data-stu-id="0d888-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d888-111">sequenceId</span><span class="sxs-lookup"><span data-stu-id="0d888-111">sequenceId</span></span> | <span data-ttu-id="0d888-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0d888-112">Int64</span></span> | <span data-ttu-id="0d888-113">DTMF イベントの順序付けに使用される増分の識別子です。</span><span class="sxs-lookup"><span data-stu-id="0d888-113">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="0d888-114">トーン</span><span class="sxs-lookup"><span data-stu-id="0d888-114">tone</span></span> | <span data-ttu-id="0d888-115">String</span><span class="sxs-lookup"><span data-stu-id="0d888-115">String</span></span> | <span data-ttu-id="0d888-116">使用可能な値: `tone0`、 `tone1`、 `tone2`、 `tone3`、 `tone4`、 `tone5`、 `tone6`、 `tone7`、 `tone8`、 `tone9`、 `star`、 `pound`、 `a`、 `b`、 `c`、 `d`、 `flash`。</span><span class="sxs-lookup"><span data-stu-id="0d888-116">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0d888-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d888-117">JSON representation</span></span>

<span data-ttu-id="0d888-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d888-118">The following is a JSON representation of the resource.</span></span>

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