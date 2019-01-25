---
title: audioSourceLevel リソースの種類
description: その他のソース レベルの構成。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528376"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="0d2f8-103">audioSourceLevel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d2f8-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d2f8-104">その他のソース レベルの構成。</span><span class="sxs-lookup"><span data-stu-id="0d2f8-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="0d2f8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d2f8-105">Properties</span></span>

| <span data-ttu-id="0d2f8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d2f8-106">Property</span></span>               | <span data-ttu-id="0d2f8-107">型</span><span class="sxs-lookup"><span data-stu-id="0d2f8-107">Type</span></span>    | <span data-ttu-id="0d2f8-108">説明</span><span class="sxs-lookup"><span data-stu-id="0d2f8-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0d2f8-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="0d2f8-109">duckOthers</span></span>             | <span data-ttu-id="0d2f8-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="0d2f8-110">Boolean</span></span> | <span data-ttu-id="0d2f8-111">Duck のアクティブなときに他のソースには、このソースを有効にします。</span><span class="sxs-lookup"><span data-stu-id="0d2f8-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="0d2f8-112">レベルをかわす、true に設定を設定する場合。</span><span class="sxs-lookup"><span data-stu-id="0d2f8-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="0d2f8-113">level</span><span class="sxs-lookup"><span data-stu-id="0d2f8-113">level</span></span>                  | <span data-ttu-id="0d2f8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0d2f8-114">Int64</span></span>   | <span data-ttu-id="0d2f8-115">場合に、ソースのレベルをかわす`duckOthers`に設定されて`true`。</span><span class="sxs-lookup"><span data-stu-id="0d2f8-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="0d2f8-116">参加者</span><span class="sxs-lookup"><span data-stu-id="0d2f8-116">participant</span></span>            | <span data-ttu-id="0d2f8-117">String</span><span class="sxs-lookup"><span data-stu-id="0d2f8-117">String</span></span>  | <span data-ttu-id="0d2f8-118">ソースの参加者オーディオ ストリームです。</span><span class="sxs-lookup"><span data-stu-id="0d2f8-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="0d2f8-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d2f8-119">JSON representation</span></span>

<span data-ttu-id="0d2f8-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d2f8-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
