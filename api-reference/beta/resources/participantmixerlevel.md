---
title: participantMixerLevel リソースの種類
description: 特定の音声参加者のミキサーレベルの構成
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 14804e02766e375568fac03cb97d2eaf76142353
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568609"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="77549-103">participantMixerLevel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77549-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77549-104">特定の音声参加者のミキサーレベルの構成</span><span class="sxs-lookup"><span data-stu-id="77549-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="77549-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77549-105">Properties</span></span>

| <span data-ttu-id="77549-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77549-106">Property</span></span>               | <span data-ttu-id="77549-107">型</span><span class="sxs-lookup"><span data-stu-id="77549-107">Type</span></span>                                                      | <span data-ttu-id="77549-108">説明</span><span class="sxs-lookup"><span data-stu-id="77549-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="77549-109">ducking</span><span class="sxs-lookup"><span data-stu-id="77549-109">ducking</span></span>                | [<span data-ttu-id="77549-110">audioアヒルの構成</span><span class="sxs-lookup"><span data-stu-id="77549-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="77549-111">この partipant カスタムミックスの他のソースの ducking (段階的なインとアウト) の構成。</span><span class="sxs-lookup"><span data-stu-id="77549-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="77549-112">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="77549-112">exclusiveMode</span></span>          | <span data-ttu-id="77549-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="77549-113">boolean</span></span>                                                   | <span data-ttu-id="77549-114">明示的なソースレベルを持たないソースをミックスから削除する必要があるかどうか。</span><span class="sxs-lookup"><span data-stu-id="77549-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="77549-115">積極的</span><span class="sxs-lookup"><span data-stu-id="77549-115">participant</span></span>            | <span data-ttu-id="77549-116">String</span><span class="sxs-lookup"><span data-stu-id="77549-116">String</span></span>                                                    | <span data-ttu-id="77549-117">ミキサーを構成する参加者。</span><span class="sxs-lookup"><span data-stu-id="77549-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="77549-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="77549-118">sourceLevels</span></span>           | <span data-ttu-id="77549-119">[audioSourceLevel](audiosourcelevel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="77549-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="77549-120">他のソースのレベルの構成。</span><span class="sxs-lookup"><span data-stu-id="77549-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="77549-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77549-121">JSON representation</span></span>

<span data-ttu-id="77549-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77549-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="77549-123">例-ミキサーレベル</span><span class="sxs-lookup"><span data-stu-id="77549-123">Example - Mixer level</span></span>

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
