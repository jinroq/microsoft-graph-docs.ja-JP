---
title: serviceHostedMediaConfig リソースの種類
description: ServiceHostedMediaConfig 型です。
author: VinodRavichandran
ms.openlocfilehash: 544c1d3bce934064092e0f9c74b888686e49d426
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380318"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="e4e18-103">serviceHostedMediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4e18-103">serviceHostedMediaConfig resource type</span></span>

> <span data-ttu-id="e4e18-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e4e18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4e18-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4e18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4e18-106">ServiceHostedMediaConfig 型です。</span><span class="sxs-lookup"><span data-stu-id="e4e18-106">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="e4e18-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4e18-107">Properties</span></span>

| <span data-ttu-id="e4e18-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4e18-108">Property</span></span>                    | <span data-ttu-id="e4e18-109">型</span><span class="sxs-lookup"><span data-stu-id="e4e18-109">Type</span></span>                                                        | <span data-ttu-id="e4e18-110">説明</span><span class="sxs-lookup"><span data-stu-id="e4e18-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="e4e18-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="e4e18-111">preFetchMedia</span></span>               | <span data-ttu-id="e4e18-112">[mediaInfo](mediainfo.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e4e18-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="e4e18-113">事前に取得するのにはメディアの一覧です。</span><span class="sxs-lookup"><span data-stu-id="e4e18-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="e4e18-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="e4e18-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="e4e18-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4e18-115">Boolean</span></span>                                                     | <span data-ttu-id="e4e18-116">オーディオの既定のグループから、自己の参加者を削除します。</span><span class="sxs-lookup"><span data-stu-id="e4e18-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e4e18-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4e18-117">JSON representation</span></span>

<span data-ttu-id="e4e18-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e4e18-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "#microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="e4e18-119">例</span><span class="sxs-lookup"><span data-stu-id="e4e18-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [
    {
      "uri": "https://cdn.contoso.com/beep.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
    },
    {
      "uri": "https://cdn.contoso.com/cool.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
    }
  ],
  "removeFromDefaultAudioGroup": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
