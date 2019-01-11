---
title: noMediaConfig リソースの種類
description: メディアがないことを示すためのメディア構成します。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c7bf75b2033c7b3340bde01b782b7eabe5ab0e76
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806462"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="5dab1-103">noMediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5dab1-103">noMediaConfig resource type</span></span>

> <span data-ttu-id="5dab1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5dab1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dab1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5dab1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5dab1-106">メディアがないことを示すためのメディア構成します。</span><span class="sxs-lookup"><span data-stu-id="5dab1-106">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="5dab1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5dab1-107">Properties</span></span>

| <span data-ttu-id="5dab1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5dab1-108">Property</span></span>       | <span data-ttu-id="5dab1-109">種類</span><span class="sxs-lookup"><span data-stu-id="5dab1-109">Type</span></span>    | <span data-ttu-id="5dab1-110">説明</span><span class="sxs-lookup"><span data-stu-id="5dab1-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5dab1-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="5dab1-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="5dab1-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="5dab1-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="5dab1-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5dab1-113">JSON representation</span></span>

<span data-ttu-id="5dab1-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5dab1-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.noMediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
