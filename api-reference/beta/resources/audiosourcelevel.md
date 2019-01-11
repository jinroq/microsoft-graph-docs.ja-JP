---
title: audioSourceLevel リソースの種類
description: その他のソース レベルの構成。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: adf3c4805271d0a8d02d25fc8e7ecb547db10215
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880641"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="7ead7-103">audioSourceLevel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7ead7-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="7ead7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ead7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ead7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ead7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ead7-106">その他のソース レベルの構成。</span><span class="sxs-lookup"><span data-stu-id="7ead7-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="7ead7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ead7-107">Properties</span></span>

| <span data-ttu-id="7ead7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ead7-108">Property</span></span>               | <span data-ttu-id="7ead7-109">種類</span><span class="sxs-lookup"><span data-stu-id="7ead7-109">Type</span></span>    | <span data-ttu-id="7ead7-110">説明</span><span class="sxs-lookup"><span data-stu-id="7ead7-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7ead7-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="7ead7-111">duckOthers</span></span>             | <span data-ttu-id="7ead7-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="7ead7-112">Boolean</span></span> | <span data-ttu-id="7ead7-113">Duck のアクティブなときに他のソースには、このソースを有効にします。</span><span class="sxs-lookup"><span data-stu-id="7ead7-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="7ead7-114">レベルをかわす、true に設定を設定する場合。</span><span class="sxs-lookup"><span data-stu-id="7ead7-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="7ead7-115">level</span><span class="sxs-lookup"><span data-stu-id="7ead7-115">level</span></span>                  | <span data-ttu-id="7ead7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7ead7-116">Int64</span></span>   | <span data-ttu-id="7ead7-117">場合に、ソースのレベルをかわす`duckOthers`に設定されて`true`。</span><span class="sxs-lookup"><span data-stu-id="7ead7-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="7ead7-118">参加者</span><span class="sxs-lookup"><span data-stu-id="7ead7-118">participant</span></span>            | <span data-ttu-id="7ead7-119">String</span><span class="sxs-lookup"><span data-stu-id="7ead7-119">String</span></span>  | <span data-ttu-id="7ead7-120">ソースの参加者オーディオ ストリームです。</span><span class="sxs-lookup"><span data-stu-id="7ead7-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="7ead7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ead7-121">JSON representation</span></span>

<span data-ttu-id="7ead7-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ead7-122">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
