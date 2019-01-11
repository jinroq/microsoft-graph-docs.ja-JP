---
title: serviceHostedMediaConfig リソースの種類
description: ServiceHostedMediaConfig 型です。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ec2ff24ef0bb45a9b49ecf2d0dc5e7419318b5af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828701"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="afe59-103">serviceHostedMediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="afe59-103">serviceHostedMediaConfig resource type</span></span>

> <span data-ttu-id="afe59-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="afe59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afe59-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afe59-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="afe59-106">ServiceHostedMediaConfig 型です。</span><span class="sxs-lookup"><span data-stu-id="afe59-106">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="afe59-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afe59-107">Properties</span></span>

| <span data-ttu-id="afe59-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afe59-108">Property</span></span>                    | <span data-ttu-id="afe59-109">種類</span><span class="sxs-lookup"><span data-stu-id="afe59-109">Type</span></span>                                                        | <span data-ttu-id="afe59-110">説明</span><span class="sxs-lookup"><span data-stu-id="afe59-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="afe59-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="afe59-111">preFetchMedia</span></span>               | <span data-ttu-id="afe59-112">[mediaInfo](mediainfo.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="afe59-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="afe59-113">事前に取得するのにはメディアの一覧です。</span><span class="sxs-lookup"><span data-stu-id="afe59-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="afe59-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="afe59-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="afe59-115">ブール型</span><span class="sxs-lookup"><span data-stu-id="afe59-115">Boolean</span></span>                                                     | <span data-ttu-id="afe59-116">オーディオの既定のグループから、自己の参加者を削除します。</span><span class="sxs-lookup"><span data-stu-id="afe59-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="afe59-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="afe59-117">JSON representation</span></span>

<span data-ttu-id="afe59-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="afe59-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="afe59-119">例</span><span class="sxs-lookup"><span data-stu-id="afe59-119">Example</span></span>

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
