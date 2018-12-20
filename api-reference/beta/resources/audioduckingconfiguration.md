---
title: audioDuckingConfiguration リソースの種類
description: ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター
author: VinodRavichandran
ms.openlocfilehash: e595e2a46f3e8bcbee2bb7ad0e3421216244db71
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380180"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="cdda8-103">audioDuckingConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cdda8-103">audioDuckingConfiguration resource type</span></span>

> <span data-ttu-id="cdda8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cdda8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdda8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdda8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cdda8-106">ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター</span><span class="sxs-lookup"><span data-stu-id="cdda8-106">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="cdda8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cdda8-107">Properties</span></span>

| <span data-ttu-id="cdda8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cdda8-108">Property</span></span>      | <span data-ttu-id="cdda8-109">型</span><span class="sxs-lookup"><span data-stu-id="cdda8-109">Type</span></span>     | <span data-ttu-id="cdda8-110">説明</span><span class="sxs-lookup"><span data-stu-id="cdda8-110">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="cdda8-111">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="cdda8-111">lowerLevel</span></span>    | <span data-ttu-id="cdda8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="cdda8-112">Int64</span></span>    | <span data-ttu-id="cdda8-113">% のソースを ducked されているときに元のボリューム。</span><span class="sxs-lookup"><span data-stu-id="cdda8-113">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="cdda8-114">rampActive</span><span class="sxs-lookup"><span data-stu-id="cdda8-114">rampActive</span></span>    | <span data-ttu-id="cdda8-115">Int64</span><span class="sxs-lookup"><span data-stu-id="cdda8-115">Int64</span></span>    | <span data-ttu-id="cdda8-116">Ducked ソースの「フェードアウト」にかかる時間 (ミリ秒単位) の量。</span><span class="sxs-lookup"><span data-stu-id="cdda8-116">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="cdda8-117">rampInactive</span><span class="sxs-lookup"><span data-stu-id="cdda8-117">rampInactive</span></span>  | <span data-ttu-id="cdda8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="cdda8-118">Int64</span></span>    | <span data-ttu-id="cdda8-119">Ducked ソースの「フェードイン」にかかる時間 (ミリ秒単位) の量。</span><span class="sxs-lookup"><span data-stu-id="cdda8-119">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="cdda8-120">upperLevel</span><span class="sxs-lookup"><span data-stu-id="cdda8-120">upperLevel</span></span>    | <span data-ttu-id="cdda8-121">Int64</span><span class="sxs-lookup"><span data-stu-id="cdda8-121">Int64</span></span>    | <span data-ttu-id="cdda8-122">% のソースは ducked されていないときに元のボリューム。</span><span class="sxs-lookup"><span data-stu-id="cdda8-122">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="cdda8-123">**注:** ランプの期間は、5,000 人以上のミリ秒になることはできません。</span><span class="sxs-lookup"><span data-stu-id="cdda8-123">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdda8-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cdda8-124">JSON representation</span></span>

<span data-ttu-id="cdda8-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cdda8-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
