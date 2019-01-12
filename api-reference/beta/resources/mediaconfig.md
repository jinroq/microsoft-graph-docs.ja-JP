---
title: mediaConfig リソースの種類
description: メディア構成は、呼び出しに接続するために使用します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 74b3b5dc4c71db80e94216756a3513a03011572a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948920"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="86eed-103">mediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86eed-103">mediaConfig resource type</span></span>

> <span data-ttu-id="86eed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86eed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86eed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86eed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86eed-106">メディア構成は、呼び出しに接続するために使用します。</span><span class="sxs-lookup"><span data-stu-id="86eed-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="86eed-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86eed-107">Properties</span></span>

| <span data-ttu-id="86eed-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86eed-108">Property</span></span>       | <span data-ttu-id="86eed-109">種類</span><span class="sxs-lookup"><span data-stu-id="86eed-109">Type</span></span>    | <span data-ttu-id="86eed-110">説明</span><span class="sxs-lookup"><span data-stu-id="86eed-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86eed-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="86eed-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="86eed-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="86eed-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="86eed-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86eed-113">JSON representation</span></span>

<span data-ttu-id="86eed-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="86eed-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "@odata.type": "microsoft.graph.mediaConfig"
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
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
