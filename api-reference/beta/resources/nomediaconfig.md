---
title: noMediaConfig リソースの種類
description: メディアがないことを示すためのメディア構成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06ca7f2c49c23575487d95bdb555d03d86860849
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573572"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="f4899-103">noMediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4899-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4899-104">メディアがないことを示すためのメディア構成します。</span><span class="sxs-lookup"><span data-stu-id="f4899-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="f4899-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4899-105">Properties</span></span>

| <span data-ttu-id="f4899-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4899-106">Property</span></span>       | <span data-ttu-id="f4899-107">型</span><span class="sxs-lookup"><span data-stu-id="f4899-107">Type</span></span>    | <span data-ttu-id="f4899-108">説明</span><span class="sxs-lookup"><span data-stu-id="f4899-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4899-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="f4899-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="f4899-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4899-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="f4899-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4899-111">JSON representation</span></span>

<span data-ttu-id="f4899-112">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4899-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.noMediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/nomediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
