---
title: mediaPrompt リソースの種類
description: MediaPrompt の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd2a700298c6f8163e3162e244f66468e1a94e7c
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932486"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="12bf2-103">mediaPrompt リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12bf2-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12bf2-104">MediaPrompt の種類。</span><span class="sxs-lookup"><span data-stu-id="12bf2-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="12bf2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12bf2-105">Properties</span></span>

| <span data-ttu-id="12bf2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12bf2-106">Property</span></span>    | <span data-ttu-id="12bf2-107">型</span><span class="sxs-lookup"><span data-stu-id="12bf2-107">Type</span></span>                      | <span data-ttu-id="12bf2-108">説明</span><span class="sxs-lookup"><span data-stu-id="12bf2-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="12bf2-109">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="12bf2-109">mediaInfo</span></span>   | [<span data-ttu-id="12bf2-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="12bf2-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="12bf2-111">メディア情報</span><span class="sxs-lookup"><span data-stu-id="12bf2-111">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="12bf2-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12bf2-112">JSON representation</span></span>

<span data-ttu-id="12bf2-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="12bf2-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="12bf2-114">例</span><span class="sxs-lookup"><span data-stu-id="12bf2-114">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "#microsoft.graph.mediaInfo",
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
