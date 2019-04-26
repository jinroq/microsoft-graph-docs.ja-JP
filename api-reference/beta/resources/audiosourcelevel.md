---
title: audioSourceLevel リソースの種類
description: 他のソースのレベルの構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc2b0c11b18a3cf8120cab0bb9c745ae8880cfc6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339064"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="642a8-103">audioSourceLevel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="642a8-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="642a8-104">他のソースのレベルの構成。</span><span class="sxs-lookup"><span data-stu-id="642a8-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="642a8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="642a8-105">Properties</span></span>

| <span data-ttu-id="642a8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="642a8-106">Property</span></span>               | <span data-ttu-id="642a8-107">型</span><span class="sxs-lookup"><span data-stu-id="642a8-107">Type</span></span>    | <span data-ttu-id="642a8-108">説明</span><span class="sxs-lookup"><span data-stu-id="642a8-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="642a8-109">その他のウィ氏</span><span class="sxs-lookup"><span data-stu-id="642a8-109">duckOthers</span></span>             | <span data-ttu-id="642a8-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="642a8-110">Boolean</span></span> | <span data-ttu-id="642a8-111">このソースが、アクティブな他のソースをアヒルに使用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="642a8-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="642a8-112">true に設定する場合は、ducking level を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="642a8-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="642a8-113">大まか</span><span class="sxs-lookup"><span data-stu-id="642a8-113">level</span></span>                  | <span data-ttu-id="642a8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="642a8-114">Int64</span></span>   | <span data-ttu-id="642a8-115">Ducking がに`true`設定され`duckOthers`ている場合のソースのレベル。</span><span class="sxs-lookup"><span data-stu-id="642a8-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="642a8-116">積極的</span><span class="sxs-lookup"><span data-stu-id="642a8-116">participant</span></span>            | <span data-ttu-id="642a8-117">String</span><span class="sxs-lookup"><span data-stu-id="642a8-117">String</span></span>  | <span data-ttu-id="642a8-118">ソース参加者のオーディオストリーム。</span><span class="sxs-lookup"><span data-stu-id="642a8-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="642a8-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="642a8-119">JSON representation</span></span>

<span data-ttu-id="642a8-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="642a8-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
