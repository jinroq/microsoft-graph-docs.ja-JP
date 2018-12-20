---
title: mediaConfig リソースの種類
description: メディア構成は、呼び出しに接続するために使用します。
author: VinodRavichandran
ms.openlocfilehash: 1b68d9236ba78ae1a83228b3382c96fc81516d1f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380262"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="3518e-103">mediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3518e-103">mediaConfig resource type</span></span>

> <span data-ttu-id="3518e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3518e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3518e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3518e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3518e-106">メディア構成は、呼び出しに接続するために使用します。</span><span class="sxs-lookup"><span data-stu-id="3518e-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="3518e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3518e-107">Properties</span></span>

| <span data-ttu-id="3518e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3518e-108">Property</span></span>       | <span data-ttu-id="3518e-109">型</span><span class="sxs-lookup"><span data-stu-id="3518e-109">Type</span></span>    | <span data-ttu-id="3518e-110">説明</span><span class="sxs-lookup"><span data-stu-id="3518e-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3518e-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="3518e-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="3518e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="3518e-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="3518e-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3518e-113">JSON representation</span></span>

<span data-ttu-id="3518e-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3518e-114">The following is a JSON representation of the resource.</span></span>

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