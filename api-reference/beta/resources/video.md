---
author: JeremyKelley
description: ビデオ リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。
ms.date: 09/10/2017
title: ビデオ
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e93fd4bbd348df3ad31d1be6aa2b1dc73593327a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007362"
---
# <a name="video-resource-type"></a><span data-ttu-id="62069-103">ビデオ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62069-103">Video resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62069-104">**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="62069-104">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="62069-p101">[**DriveItem**](driveitem.md) に null 以外の**ビデオ** ファセットがある場合は、項目はビデオ ファイルを表します。**ビデオ** リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。</span><span class="sxs-lookup"><span data-stu-id="62069-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62069-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62069-107">JSON representation</span></span>

<span data-ttu-id="62069-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="62069-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "height": 1280,
  "width": 720,
  "framerate": 2.75
}
```

## <a name="properties"></a><span data-ttu-id="62069-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62069-109">Properties</span></span>

| <span data-ttu-id="62069-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="62069-110">Property name</span></span>             | <span data-ttu-id="62069-111">種類</span><span class="sxs-lookup"><span data-stu-id="62069-111">Type</span></span>   | <span data-ttu-id="62069-112">説明</span><span class="sxs-lookup"><span data-stu-id="62069-112">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="62069-113">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="62069-113">**audioBitsPerSample**</span></span>    | <span data-ttu-id="62069-114">Int32</span><span class="sxs-lookup"><span data-stu-id="62069-114">Int32</span></span>  | <span data-ttu-id="62069-115">サンプルあたりのオーディオ ビット数。</span><span class="sxs-lookup"><span data-stu-id="62069-115">Number of audio bits per sample.</span></span>
| <span data-ttu-id="62069-116">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="62069-116">**audioChannels**</span></span>         | <span data-ttu-id="62069-117">Int32</span><span class="sxs-lookup"><span data-stu-id="62069-117">Int32</span></span>  | <span data-ttu-id="62069-118">オーディオ チャンネル数。</span><span class="sxs-lookup"><span data-stu-id="62069-118">Number of audio channels.</span></span>
| <span data-ttu-id="62069-119">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="62069-119">**audioFormat**</span></span>           | <span data-ttu-id="62069-120">string</span><span class="sxs-lookup"><span data-stu-id="62069-120">string</span></span> | <span data-ttu-id="62069-121">オーディオ形式の名前 (AAC、MP3 など)。</span><span class="sxs-lookup"><span data-stu-id="62069-121">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="62069-122">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="62069-122">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="62069-123">Int32</span><span class="sxs-lookup"><span data-stu-id="62069-123">Int32</span></span>  | <span data-ttu-id="62069-124">1 秒あたりのオーディオ サンプル数。</span><span class="sxs-lookup"><span data-stu-id="62069-124">Number of audio samples per second.</span></span>
| <span data-ttu-id="62069-125">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="62069-125">**bitrate**</span></span>               | <span data-ttu-id="62069-126">Int32</span><span class="sxs-lookup"><span data-stu-id="62069-126">Int32</span></span>  | <span data-ttu-id="62069-127">1 秒あたりのビデオのビット レート (ビット単位)。</span><span class="sxs-lookup"><span data-stu-id="62069-127">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="62069-128">**duration**</span><span class="sxs-lookup"><span data-stu-id="62069-128">**duration**</span></span>              | <span data-ttu-id="62069-129">Int64</span><span class="sxs-lookup"><span data-stu-id="62069-129">Int64</span></span>  | <span data-ttu-id="62069-130">ファイルの継続時間 (ミリ秒単位)。</span><span class="sxs-lookup"><span data-stu-id="62069-130">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="62069-131">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="62069-131">**fourCC**</span></span>                | <span data-ttu-id="62069-132">string</span><span class="sxs-lookup"><span data-stu-id="62069-132">string</span></span> | <span data-ttu-id="62069-133">ビデオ形式の「4 文字コード」名。</span><span class="sxs-lookup"><span data-stu-id="62069-133">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="62069-134">**framerate**</span><span class="sxs-lookup"><span data-stu-id="62069-134">**framerate**</span></span>             | <span data-ttu-id="62069-135">double</span><span class="sxs-lookup"><span data-stu-id="62069-135">double</span></span> | <span data-ttu-id="62069-136">ビデオのフレーム レート。</span><span class="sxs-lookup"><span data-stu-id="62069-136">Frame rate of the video.</span></span>
| <span data-ttu-id="62069-137">**height**</span><span class="sxs-lookup"><span data-stu-id="62069-137">**height**</span></span>                | <span data-ttu-id="62069-138">Int32</span><span class="sxs-lookup"><span data-stu-id="62069-138">Int32</span></span>  | <span data-ttu-id="62069-139">ビデオの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="62069-139">Height of the video, in pixels.</span></span>
| <span data-ttu-id="62069-140">**width**</span><span class="sxs-lookup"><span data-stu-id="62069-140">**width**</span></span>                 | <span data-ttu-id="62069-141">Int32</span><span class="sxs-lookup"><span data-stu-id="62069-141">Int32</span></span>  | <span data-ttu-id="62069-142">ビデオの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="62069-142">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="62069-143">注釈</span><span class="sxs-lookup"><span data-stu-id="62069-143">Remarks</span></span>

<span data-ttu-id="62069-144">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62069-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
