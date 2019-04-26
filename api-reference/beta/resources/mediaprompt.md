---
title: mediaprompt リソースの種類
description: mediaprompt の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b87af39d6d6ac4879aba44573b920a43d4f92145
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562596"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="2b65b-103">mediaprompt リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b65b-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b65b-104">mediaprompt の種類。</span><span class="sxs-lookup"><span data-stu-id="2b65b-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="2b65b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b65b-105">Properties</span></span>

| <span data-ttu-id="2b65b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b65b-106">Property</span></span>    | <span data-ttu-id="2b65b-107">型</span><span class="sxs-lookup"><span data-stu-id="2b65b-107">Type</span></span>                      | <span data-ttu-id="2b65b-108">説明</span><span class="sxs-lookup"><span data-stu-id="2b65b-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="2b65b-109">for</span><span class="sxs-lookup"><span data-stu-id="2b65b-109">loop</span></span>        | <span data-ttu-id="2b65b-110">Int32</span><span class="sxs-lookup"><span data-stu-id="2b65b-110">Int32</span></span>                     | <span data-ttu-id="2b65b-111">ループカウント。</span><span class="sxs-lookup"><span data-stu-id="2b65b-111">The loop count.</span></span> <span data-ttu-id="2b65b-112">0は無限にループすることを示します。</span><span class="sxs-lookup"><span data-stu-id="2b65b-112">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="2b65b-113">既定値は `1` です。</span><span class="sxs-lookup"><span data-stu-id="2b65b-113">The default value is `1`.</span></span> |
| <span data-ttu-id="2b65b-114">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2b65b-114">mediaInfo</span></span>   | [<span data-ttu-id="2b65b-115">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2b65b-115">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="2b65b-116">メディア情報</span><span class="sxs-lookup"><span data-stu-id="2b65b-116">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="2b65b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b65b-117">JSON representation</span></span>

<span data-ttu-id="2b65b-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b65b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="2b65b-119">例</span><span class="sxs-lookup"><span data-stu-id="2b65b-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
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
