---
title: participantMixerLevel リソースの種類
description: 特定の参加者のオーディオのをレベルをミキサーの設定
author: VinodRavichandran
ms.openlocfilehash: 9d5a5d740fbdf250f90b28539221e8231c0bf38c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380143"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="b1042-103">participantMixerLevel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1042-103">participantMixerLevel resource type</span></span>

> <span data-ttu-id="b1042-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1042-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1042-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1042-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1042-106">特定の参加者のオーディオのをレベルをミキサーの設定</span><span class="sxs-lookup"><span data-stu-id="b1042-106">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="b1042-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1042-107">Properties</span></span>

| <span data-ttu-id="b1042-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1042-108">Property</span></span>               | <span data-ttu-id="b1042-109">型</span><span class="sxs-lookup"><span data-stu-id="b1042-109">Type</span></span>                                                      | <span data-ttu-id="b1042-110">説明</span><span class="sxs-lookup"><span data-stu-id="b1042-110">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b1042-111">ダック</span><span class="sxs-lookup"><span data-stu-id="b1042-111">ducking</span></span>                | [<span data-ttu-id="b1042-112">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1042-112">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="b1042-113">ダック (段階的に導入と出力) のこの partipant の他のソースのカスタム ミックスの構成です。</span><span class="sxs-lookup"><span data-stu-id="b1042-113">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="b1042-114">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="b1042-114">exclusiveMode</span></span>          | <span data-ttu-id="b1042-115">ブール</span><span class="sxs-lookup"><span data-stu-id="b1042-115">boolean</span></span>                                                   | <span data-ttu-id="b1042-116">かどうか、ミックスから明示的なソース レベルのないソースを削除してください。</span><span class="sxs-lookup"><span data-stu-id="b1042-116">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="b1042-117">参加者</span><span class="sxs-lookup"><span data-stu-id="b1042-117">participant</span></span>            | <span data-ttu-id="b1042-118">String</span><span class="sxs-lookup"><span data-stu-id="b1042-118">String</span></span>                                                    | <span data-ttu-id="b1042-119">ミキサーが構成されている構成要素です。</span><span class="sxs-lookup"><span data-stu-id="b1042-119">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="b1042-120">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="b1042-120">sourceLevels</span></span>           | <span data-ttu-id="b1042-121">[audioSourceLevel](audiosourcelevel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b1042-121">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="b1042-122">その他のソース レベルの構成。</span><span class="sxs-lookup"><span data-stu-id="b1042-122">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="b1042-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1042-123">JSON representation</span></span>

<span data-ttu-id="b1042-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b1042-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "#microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "#microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a><span data-ttu-id="b1042-125">ミキサー レベルの使用例</span><span class="sxs-lookup"><span data-stu-id="b1042-125">Example - Mixer level</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": {
    "@odata.type": "#microsoft.graph.audioDuckingParameters",
    "rampActive": 1000,
    "rampInactive": 1000,
    "lowerLevel": 20,
    "upperLevel": 100
  },
  "exclusiveMode": true,
  "participant": "123456W77E24E4D85F80597083CB830",
  "sourceLevels": [
    {
      "@odata.type": "#microsoft.graph.audioSourceLevel",
      "duckOthers": false,
      "level": 100,
      "participant": "8A34A46B3D174ADC8DCEDC4E7D572698"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
