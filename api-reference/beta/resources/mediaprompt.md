---
title: mediaPrompt リソースの種類
description: MediaPrompt 型です。
author: VinodRavichandran
ms.openlocfilehash: 4782772f463a613a759ad3b2b25cb05e7e160555
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380290"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="2cd65-103">mediaPrompt リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2cd65-103">mediaPrompt resource type</span></span>

> <span data-ttu-id="2cd65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2cd65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cd65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cd65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2cd65-106">MediaPrompt 型です。</span><span class="sxs-lookup"><span data-stu-id="2cd65-106">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="2cd65-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cd65-107">Properties</span></span>

| <span data-ttu-id="2cd65-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cd65-108">Property</span></span>    | <span data-ttu-id="2cd65-109">型</span><span class="sxs-lookup"><span data-stu-id="2cd65-109">Type</span></span>                      | <span data-ttu-id="2cd65-110">説明</span><span class="sxs-lookup"><span data-stu-id="2cd65-110">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="2cd65-111">ループ</span><span class="sxs-lookup"><span data-stu-id="2cd65-111">loop</span></span>        | <span data-ttu-id="2cd65-112">Int32</span><span class="sxs-lookup"><span data-stu-id="2cd65-112">Int32</span></span>                     | <span data-ttu-id="2cd65-113">ループ カウントです。</span><span class="sxs-lookup"><span data-stu-id="2cd65-113">The loop count.</span></span> <span data-ttu-id="2cd65-114">値 0 は、無限にループすることを示します。</span><span class="sxs-lookup"><span data-stu-id="2cd65-114">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="2cd65-115">既定値は、 `1`。</span><span class="sxs-lookup"><span data-stu-id="2cd65-115">The default value is `1`.</span></span> |
| <span data-ttu-id="2cd65-116">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2cd65-116">mediaInfo</span></span>   | [<span data-ttu-id="2cd65-117">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2cd65-117">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="2cd65-118">メディア情報</span><span class="sxs-lookup"><span data-stu-id="2cd65-118">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="2cd65-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cd65-119">JSON representation</span></span>

<span data-ttu-id="2cd65-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2cd65-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="2cd65-121">例</span><span class="sxs-lookup"><span data-stu-id="2cd65-121">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
