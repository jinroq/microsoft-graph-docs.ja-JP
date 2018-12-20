---
title: noMediaConfig リソースの種類
description: メディアがないことを示すためのメディア構成します。
author: VinodRavichandran
ms.openlocfilehash: 29d5230150a035d8ed2dd1223f66df4a8f4f30f2
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380184"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="bf6be-103">noMediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf6be-103">noMediaConfig resource type</span></span>

> <span data-ttu-id="bf6be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf6be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf6be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf6be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf6be-106">メディアがないことを示すためのメディア構成します。</span><span class="sxs-lookup"><span data-stu-id="bf6be-106">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="bf6be-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf6be-107">Properties</span></span>

| <span data-ttu-id="bf6be-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf6be-108">Property</span></span>       | <span data-ttu-id="bf6be-109">型</span><span class="sxs-lookup"><span data-stu-id="bf6be-109">Type</span></span>    | <span data-ttu-id="bf6be-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf6be-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf6be-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="bf6be-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="bf6be-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf6be-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="bf6be-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf6be-113">JSON representation</span></span>

<span data-ttu-id="bf6be-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bf6be-114">The following is a JSON representation of the resource.</span></span>

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
