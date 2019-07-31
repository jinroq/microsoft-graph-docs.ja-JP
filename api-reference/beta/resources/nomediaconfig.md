---
title: noMediaConfig リソースの種類
description: メディアがないことを示すためのメディア構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 97d2ac01b434e211eb8836f04343ef65b9f0ea1b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966665"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="91347-103">noMediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91347-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91347-104">メディアがないことを示すためのメディア構成。</span><span class="sxs-lookup"><span data-stu-id="91347-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="91347-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91347-105">Properties</span></span>

| <span data-ttu-id="91347-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91347-106">Property</span></span>       | <span data-ttu-id="91347-107">型</span><span class="sxs-lookup"><span data-stu-id="91347-107">Type</span></span>    | <span data-ttu-id="91347-108">説明</span><span class="sxs-lookup"><span data-stu-id="91347-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91347-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="91347-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="91347-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="91347-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="91347-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91347-111">JSON representation</span></span>

<span data-ttu-id="91347-112">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91347-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
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
  "suppressions": []
}
-->
