---
title: audioDuckingConfiguration リソースの種類
description: ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d61e4150250df25e020f45a65676d1c55c0e4c9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522463"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="8bb03-103">audioDuckingConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8bb03-103">audioDuckingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb03-104">ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター</span><span class="sxs-lookup"><span data-stu-id="8bb03-104">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="8bb03-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bb03-105">Properties</span></span>

| <span data-ttu-id="8bb03-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bb03-106">Property</span></span>      | <span data-ttu-id="8bb03-107">型</span><span class="sxs-lookup"><span data-stu-id="8bb03-107">Type</span></span>     | <span data-ttu-id="8bb03-108">説明</span><span class="sxs-lookup"><span data-stu-id="8bb03-108">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="8bb03-109">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="8bb03-109">lowerLevel</span></span>    | <span data-ttu-id="8bb03-110">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb03-110">Int64</span></span>    | <span data-ttu-id="8bb03-111">% のソースを ducked されているときに元のボリューム。</span><span class="sxs-lookup"><span data-stu-id="8bb03-111">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="8bb03-112">rampActive</span><span class="sxs-lookup"><span data-stu-id="8bb03-112">rampActive</span></span>    | <span data-ttu-id="8bb03-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb03-113">Int64</span></span>    | <span data-ttu-id="8bb03-114">Ducked ソースの「フェードアウト」にかかる時間 (ミリ秒単位) の量。</span><span class="sxs-lookup"><span data-stu-id="8bb03-114">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="8bb03-115">rampInactive</span><span class="sxs-lookup"><span data-stu-id="8bb03-115">rampInactive</span></span>  | <span data-ttu-id="8bb03-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb03-116">Int64</span></span>    | <span data-ttu-id="8bb03-117">Ducked ソースの「フェードイン」にかかる時間 (ミリ秒単位) の量。</span><span class="sxs-lookup"><span data-stu-id="8bb03-117">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="8bb03-118">upperLevel</span><span class="sxs-lookup"><span data-stu-id="8bb03-118">upperLevel</span></span>    | <span data-ttu-id="8bb03-119">Int64</span><span class="sxs-lookup"><span data-stu-id="8bb03-119">Int64</span></span>    | <span data-ttu-id="8bb03-120">% のソースは ducked されていないときに元のボリューム。</span><span class="sxs-lookup"><span data-stu-id="8bb03-120">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="8bb03-121">**注:** ランプの期間は、5,000 人以上のミリ秒になることはできません。</span><span class="sxs-lookup"><span data-stu-id="8bb03-121">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bb03-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8bb03-122">JSON representation</span></span>

<span data-ttu-id="8bb03-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bb03-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioduckingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
