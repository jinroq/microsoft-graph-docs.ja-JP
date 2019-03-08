---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ビデオ
localization_priority: Normal
ms.openlocfilehash: deba8cccb5f0ab80ca03395ef9f798719d542b8d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480804"
---
# <a name="video-resource-type"></a><span data-ttu-id="5542f-102">ビデオ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5542f-102">Video resource type</span></span>

<span data-ttu-id="5542f-103">**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="5542f-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="5542f-p101">[**DriveItem**](driveitem.md) に null 以外の**ビデオ** ファセットがある場合は、項目はビデオ ファイルを表します。**ビデオ** リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。</span><span class="sxs-lookup"><span data-stu-id="5542f-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5542f-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5542f-106">JSON representation</span></span>

<span data-ttu-id="5542f-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="5542f-107">Here is a JSON representation of the resource</span></span>

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
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a><span data-ttu-id="5542f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5542f-108">Properties</span></span>

| <span data-ttu-id="5542f-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="5542f-109">Property name</span></span>             | <span data-ttu-id="5542f-110">種類</span><span class="sxs-lookup"><span data-stu-id="5542f-110">Type</span></span>   | <span data-ttu-id="5542f-111">説明</span><span class="sxs-lookup"><span data-stu-id="5542f-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="5542f-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="5542f-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="5542f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5542f-113">Int32</span></span>  | <span data-ttu-id="5542f-114">サンプルあたりのオーディオ ビット数。</span><span class="sxs-lookup"><span data-stu-id="5542f-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="5542f-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="5542f-115">**audioChannels**</span></span>         | <span data-ttu-id="5542f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5542f-116">Int32</span></span>  | <span data-ttu-id="5542f-117">オーディオ チャンネル数。</span><span class="sxs-lookup"><span data-stu-id="5542f-117">Number of audio channels.</span></span>
| <span data-ttu-id="5542f-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="5542f-118">**audioFormat**</span></span>           | <span data-ttu-id="5542f-119">string</span><span class="sxs-lookup"><span data-stu-id="5542f-119">string</span></span> | <span data-ttu-id="5542f-120">オーディオ形式の名前 (AAC、MP3 など)。</span><span class="sxs-lookup"><span data-stu-id="5542f-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="5542f-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="5542f-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="5542f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="5542f-122">Int32</span></span>  | <span data-ttu-id="5542f-123">1 秒あたりのオーディオ サンプル数。</span><span class="sxs-lookup"><span data-stu-id="5542f-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="5542f-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="5542f-124">**bitrate**</span></span>               | <span data-ttu-id="5542f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="5542f-125">Int32</span></span>  | <span data-ttu-id="5542f-126">1 秒あたりのビデオのビット レート (ビット単位)。</span><span class="sxs-lookup"><span data-stu-id="5542f-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="5542f-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="5542f-127">**duration**</span></span>              | <span data-ttu-id="5542f-128">Int64</span><span class="sxs-lookup"><span data-stu-id="5542f-128">Int64</span></span>  | <span data-ttu-id="5542f-129">ファイルの継続時間 (ミリ秒単位)。</span><span class="sxs-lookup"><span data-stu-id="5542f-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="5542f-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="5542f-130">**fourCC**</span></span>                | <span data-ttu-id="5542f-131">string</span><span class="sxs-lookup"><span data-stu-id="5542f-131">string</span></span> | <span data-ttu-id="5542f-132">ビデオ形式の「4 文字コード」名。</span><span class="sxs-lookup"><span data-stu-id="5542f-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="5542f-133">**frameRate**</span><span class="sxs-lookup"><span data-stu-id="5542f-133">**frameRate**</span></span>             | <span data-ttu-id="5542f-134">double</span><span class="sxs-lookup"><span data-stu-id="5542f-134">double</span></span> | <span data-ttu-id="5542f-135">ビデオのフレーム レート。</span><span class="sxs-lookup"><span data-stu-id="5542f-135">Frame rate of the video.</span></span>
| <span data-ttu-id="5542f-136">**height**</span><span class="sxs-lookup"><span data-stu-id="5542f-136">**height**</span></span>                | <span data-ttu-id="5542f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5542f-137">Int32</span></span>  | <span data-ttu-id="5542f-138">ビデオの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="5542f-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="5542f-139">**width**</span><span class="sxs-lookup"><span data-stu-id="5542f-139">**width**</span></span>                 | <span data-ttu-id="5542f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5542f-140">Int32</span></span>  | <span data-ttu-id="5542f-141">ビデオの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="5542f-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="5542f-142">注釈</span><span class="sxs-lookup"><span data-stu-id="5542f-142">Remarks</span></span>

<span data-ttu-id="5542f-143">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5542f-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
