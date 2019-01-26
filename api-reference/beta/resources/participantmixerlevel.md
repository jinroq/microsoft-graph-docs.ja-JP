---
title: participantMixerLevel リソースの種類
description: 特定の参加者のオーディオのをレベルをミキサーの設定
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb5d28ac45d510a715dcc5001c8ee02b8352bb8c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575420"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="6a50a-103">participantMixerLevel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a50a-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a50a-104">特定の参加者のオーディオのをレベルをミキサーの設定</span><span class="sxs-lookup"><span data-stu-id="6a50a-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="6a50a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a50a-105">Properties</span></span>

| <span data-ttu-id="6a50a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a50a-106">Property</span></span>               | <span data-ttu-id="6a50a-107">型</span><span class="sxs-lookup"><span data-stu-id="6a50a-107">Type</span></span>                                                      | <span data-ttu-id="6a50a-108">説明</span><span class="sxs-lookup"><span data-stu-id="6a50a-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6a50a-109">ダック</span><span class="sxs-lookup"><span data-stu-id="6a50a-109">ducking</span></span>                | [<span data-ttu-id="6a50a-110">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a50a-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="6a50a-111">ダック (段階的に導入と出力) のこの partipant の他のソースのカスタム ミックスの構成です。</span><span class="sxs-lookup"><span data-stu-id="6a50a-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="6a50a-112">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="6a50a-112">exclusiveMode</span></span>          | <span data-ttu-id="6a50a-113">boolean</span><span class="sxs-lookup"><span data-stu-id="6a50a-113">boolean</span></span>                                                   | <span data-ttu-id="6a50a-114">かどうか、ミックスから明示的なソース レベルのないソースを削除してください。</span><span class="sxs-lookup"><span data-stu-id="6a50a-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="6a50a-115">参加者</span><span class="sxs-lookup"><span data-stu-id="6a50a-115">participant</span></span>            | <span data-ttu-id="6a50a-116">String</span><span class="sxs-lookup"><span data-stu-id="6a50a-116">String</span></span>                                                    | <span data-ttu-id="6a50a-117">ミキサーが構成されている構成要素です。</span><span class="sxs-lookup"><span data-stu-id="6a50a-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="6a50a-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="6a50a-118">sourceLevels</span></span>           | <span data-ttu-id="6a50a-119">[audioSourceLevel](audiosourcelevel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6a50a-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="6a50a-120">その他のソース レベルの構成。</span><span class="sxs-lookup"><span data-stu-id="6a50a-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="6a50a-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a50a-121">JSON representation</span></span>

<span data-ttu-id="6a50a-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a50a-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a><span data-ttu-id="6a50a-123">ミキサー レベルの使用例</span><span class="sxs-lookup"><span data-stu-id="6a50a-123">Example - Mixer level</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participantmixerlevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
