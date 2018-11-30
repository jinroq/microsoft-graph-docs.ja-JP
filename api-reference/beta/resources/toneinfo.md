---
title: toneInfo リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: b4ed9667c2e2156f52703c6fa15f4937ead5cef4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073773"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="121ce-103">toneInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="121ce-103">toneInfo resource type</span></span>

> <span data-ttu-id="121ce-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="121ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="121ce-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="121ce-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="121ce-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="121ce-106">Properties</span></span>

| <span data-ttu-id="121ce-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="121ce-107">Property</span></span>       | <span data-ttu-id="121ce-108">型</span><span class="sxs-lookup"><span data-stu-id="121ce-108">Type</span></span>    | <span data-ttu-id="121ce-109">説明</span><span class="sxs-lookup"><span data-stu-id="121ce-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="121ce-110">sequenceId</span><span class="sxs-lookup"><span data-stu-id="121ce-110">sequenceId</span></span> | <span data-ttu-id="121ce-111">Int64</span><span class="sxs-lookup"><span data-stu-id="121ce-111">Int64</span></span> | <span data-ttu-id="121ce-112">DTMF イベントの順序付けに使用される増分の識別子です。</span><span class="sxs-lookup"><span data-stu-id="121ce-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="121ce-113">トーン</span><span class="sxs-lookup"><span data-stu-id="121ce-113">tone</span></span> | <span data-ttu-id="121ce-114">String</span><span class="sxs-lookup"><span data-stu-id="121ce-114">String</span></span> | <span data-ttu-id="121ce-115">使用可能な値: `tone0`、 `tone1`、 `tone2`、 `tone3`、 `tone4`、 `tone5`、 `tone6`、 `tone7`、 `tone8`、 `tone9`、 `star`、 `pound`、 `a`、 `b`、 `c`、 `d`、 `flash`。</span><span class="sxs-lookup"><span data-stu-id="121ce-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="121ce-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="121ce-116">JSON representation</span></span>

<span data-ttu-id="121ce-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="121ce-117">The following is a JSON representation of the resource.</span></span>

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