---
title: audioDuckingConfiguration リソースの種類
description: ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4132946573342976bb1f20c593454a8e18030d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916874"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="64762-103">audioDuckingConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64762-103">audioDuckingConfiguration resource type</span></span>

> <span data-ttu-id="64762-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="64762-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64762-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64762-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64762-106">ダック (その他のソースとの間でフェードアウト) の他のソースのためのパラメーター</span><span class="sxs-lookup"><span data-stu-id="64762-106">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="64762-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64762-107">Properties</span></span>

| <span data-ttu-id="64762-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64762-108">Property</span></span>      | <span data-ttu-id="64762-109">種類</span><span class="sxs-lookup"><span data-stu-id="64762-109">Type</span></span>     | <span data-ttu-id="64762-110">説明</span><span class="sxs-lookup"><span data-stu-id="64762-110">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="64762-111">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="64762-111">lowerLevel</span></span>    | <span data-ttu-id="64762-112">Int64</span><span class="sxs-lookup"><span data-stu-id="64762-112">Int64</span></span>    | <span data-ttu-id="64762-113">% のソースを ducked されているときに元のボリューム。</span><span class="sxs-lookup"><span data-stu-id="64762-113">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="64762-114">rampActive</span><span class="sxs-lookup"><span data-stu-id="64762-114">rampActive</span></span>    | <span data-ttu-id="64762-115">Int64</span><span class="sxs-lookup"><span data-stu-id="64762-115">Int64</span></span>    | <span data-ttu-id="64762-116">Ducked ソースの「フェードアウト」にかかる時間 (ミリ秒単位) の量。</span><span class="sxs-lookup"><span data-stu-id="64762-116">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="64762-117">rampInactive</span><span class="sxs-lookup"><span data-stu-id="64762-117">rampInactive</span></span>  | <span data-ttu-id="64762-118">Int64</span><span class="sxs-lookup"><span data-stu-id="64762-118">Int64</span></span>    | <span data-ttu-id="64762-119">Ducked ソースの「フェードイン」にかかる時間 (ミリ秒単位) の量。</span><span class="sxs-lookup"><span data-stu-id="64762-119">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="64762-120">upperLevel</span><span class="sxs-lookup"><span data-stu-id="64762-120">upperLevel</span></span>    | <span data-ttu-id="64762-121">Int64</span><span class="sxs-lookup"><span data-stu-id="64762-121">Int64</span></span>    | <span data-ttu-id="64762-122">% のソースは ducked されていないときに元のボリューム。</span><span class="sxs-lookup"><span data-stu-id="64762-122">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="64762-123">**注:** ランプの期間は、5,000 人以上のミリ秒になることはできません。</span><span class="sxs-lookup"><span data-stu-id="64762-123">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64762-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64762-124">JSON representation</span></span>

<span data-ttu-id="64762-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64762-125">The following is a JSON representation of the resource.</span></span>

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
