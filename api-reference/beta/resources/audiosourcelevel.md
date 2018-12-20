---
title: audioSourceLevel リソースの種類
description: その他のソース レベルの構成。
author: VinodRavichandran
ms.openlocfilehash: 5d5abe7eba03891427b30ba1c8f63b15b3707e46
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380241"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="b431b-103">audioSourceLevel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b431b-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="b431b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b431b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b431b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b431b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b431b-106">その他のソース レベルの構成。</span><span class="sxs-lookup"><span data-stu-id="b431b-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="b431b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b431b-107">Properties</span></span>

| <span data-ttu-id="b431b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b431b-108">Property</span></span>               | <span data-ttu-id="b431b-109">型</span><span class="sxs-lookup"><span data-stu-id="b431b-109">Type</span></span>    | <span data-ttu-id="b431b-110">説明</span><span class="sxs-lookup"><span data-stu-id="b431b-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b431b-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="b431b-111">duckOthers</span></span>             | <span data-ttu-id="b431b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b431b-112">Boolean</span></span> | <span data-ttu-id="b431b-113">Duck のアクティブなときに他のソースには、このソースを有効にします。</span><span class="sxs-lookup"><span data-stu-id="b431b-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="b431b-114">レベルをかわす、true に設定を設定する場合。</span><span class="sxs-lookup"><span data-stu-id="b431b-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="b431b-115">level</span><span class="sxs-lookup"><span data-stu-id="b431b-115">level</span></span>                  | <span data-ttu-id="b431b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b431b-116">Int64</span></span>   | <span data-ttu-id="b431b-117">場合に、ソースのレベルをかわす`duckOthers`に設定されて`true`。</span><span class="sxs-lookup"><span data-stu-id="b431b-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="b431b-118">参加者</span><span class="sxs-lookup"><span data-stu-id="b431b-118">participant</span></span>            | <span data-ttu-id="b431b-119">String</span><span class="sxs-lookup"><span data-stu-id="b431b-119">String</span></span>  | <span data-ttu-id="b431b-120">ソースの参加者オーディオ ストリームです。</span><span class="sxs-lookup"><span data-stu-id="b431b-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="b431b-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b431b-121">JSON representation</span></span>

<span data-ttu-id="b431b-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b431b-122">The following is a JSON representation of the resource.</span></span>

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
