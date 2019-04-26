---
title: noMediaConfig リソースの種類
description: メディアがないことを示すためのメディア構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ec1c70e233f46ad0098a6a7ee76d4d46f3b82c20
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342157"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="4e3ed-103">noMediaConfig リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e3ed-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e3ed-104">メディアがないことを示すためのメディア構成。</span><span class="sxs-lookup"><span data-stu-id="4e3ed-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="4e3ed-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e3ed-105">Properties</span></span>

| <span data-ttu-id="4e3ed-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e3ed-106">Property</span></span>       | <span data-ttu-id="4e3ed-107">型</span><span class="sxs-lookup"><span data-stu-id="4e3ed-107">Type</span></span>    | <span data-ttu-id="4e3ed-108">説明</span><span class="sxs-lookup"><span data-stu-id="4e3ed-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4e3ed-109">removefromdefaultaudiogroup</span><span class="sxs-lookup"><span data-stu-id="4e3ed-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="4e3ed-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e3ed-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="4e3ed-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e3ed-111">JSON representation</span></span>

<span data-ttu-id="4e3ed-112">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4e3ed-112">The following is a JSON representation of the resource.</span></span>

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
