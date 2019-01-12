---
title: noMediaConfig リソースの種類
description: メディアがないことを示すためのメディア構成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 64ab5c5bb6cbff6d9af677be9c85c13bfcd78d75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983388"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="1d658-103">noMediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d658-103">noMediaConfig resource type</span></span>

> <span data-ttu-id="1d658-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d658-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d658-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d658-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d658-106">メディアがないことを示すためのメディア構成します。</span><span class="sxs-lookup"><span data-stu-id="1d658-106">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="1d658-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d658-107">Properties</span></span>

| <span data-ttu-id="1d658-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d658-108">Property</span></span>       | <span data-ttu-id="1d658-109">種類</span><span class="sxs-lookup"><span data-stu-id="1d658-109">Type</span></span>    | <span data-ttu-id="1d658-110">説明</span><span class="sxs-lookup"><span data-stu-id="1d658-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d658-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="1d658-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="1d658-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="1d658-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="1d658-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d658-113">JSON representation</span></span>

<span data-ttu-id="1d658-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d658-114">The following is a JSON representation of the resource.</span></span>

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
