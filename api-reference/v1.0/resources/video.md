---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: dd6ece46ce54fe791c0e6b5801287e2abad4fe48
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="video-resource-type"></a><span data-ttu-id="3af3a-102">Video リソース型</span><span class="sxs-lookup"><span data-stu-id="3af3a-102">Video resource type</span></span>

<span data-ttu-id="3af3a-103">**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="3af3a-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="3af3a-104">[**DriveItem**](driveitem.md) に null でない **video** ファセットがある場合、そのアイテムはビデオ ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="3af3a-104">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the Video resource are populated by extracting metadata from the file.</span></span>
<span data-ttu-id="3af3a-105">**Video** リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。</span><span class="sxs-lookup"><span data-stu-id="3af3a-105">If a DriveItem has a non-null video facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3af3a-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3af3a-106">JSON representation</span></span>

<span data-ttu-id="3af3a-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3af3a-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3af3a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3af3a-108">Properties</span></span>

| <span data-ttu-id="3af3a-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="3af3a-109">Property name</span></span>             | <span data-ttu-id="3af3a-110">種類</span><span class="sxs-lookup"><span data-stu-id="3af3a-110">Type</span></span>   | <span data-ttu-id="3af3a-111">説明</span><span class="sxs-lookup"><span data-stu-id="3af3a-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="3af3a-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="3af3a-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="3af3a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3af3a-113">Int32</span></span>  | <span data-ttu-id="3af3a-114">1 サンプルあたりのオーディオ ビット数。</span><span class="sxs-lookup"><span data-stu-id="3af3a-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="3af3a-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="3af3a-115">**audioChannels**</span></span>         | <span data-ttu-id="3af3a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3af3a-116">Int32</span></span>  | <span data-ttu-id="3af3a-117">オーディオ チャンネル数。</span><span class="sxs-lookup"><span data-stu-id="3af3a-117">Number of audio channels.</span></span>
| <span data-ttu-id="3af3a-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="3af3a-118">**audioFormat**</span></span>           | <span data-ttu-id="3af3a-119">string</span><span class="sxs-lookup"><span data-stu-id="3af3a-119">string</span></span> | <span data-ttu-id="3af3a-120">オーディオ形式の名前 (AAC、MP3 など)。</span><span class="sxs-lookup"><span data-stu-id="3af3a-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="3af3a-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="3af3a-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="3af3a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3af3a-122">Int32</span></span>  | <span data-ttu-id="3af3a-123">1 秒あたりのオーディオ サンプル数。</span><span class="sxs-lookup"><span data-stu-id="3af3a-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="3af3a-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="3af3a-124">**bitrate**</span></span>               | <span data-ttu-id="3af3a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3af3a-125">Int32</span></span>  | <span data-ttu-id="3af3a-126">1 秒あたりのビデオのビット レート (ビット単位)。</span><span class="sxs-lookup"><span data-stu-id="3af3a-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="3af3a-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="3af3a-127">**duration**</span></span>              | <span data-ttu-id="3af3a-128">Int64</span><span class="sxs-lookup"><span data-stu-id="3af3a-128">Int64</span></span>  | <span data-ttu-id="3af3a-129">ファイルの長さ (ミリ秒単位)。</span><span class="sxs-lookup"><span data-stu-id="3af3a-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="3af3a-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="3af3a-130">**fourCC**</span></span>                | <span data-ttu-id="3af3a-131">string</span><span class="sxs-lookup"><span data-stu-id="3af3a-131">string</span></span> | <span data-ttu-id="3af3a-132">ビデオ形式の「4 文字コード」名。</span><span class="sxs-lookup"><span data-stu-id="3af3a-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="3af3a-133">**framerate**</span><span class="sxs-lookup"><span data-stu-id="3af3a-133">**framerate**</span></span>             | <span data-ttu-id="3af3a-134">double</span><span class="sxs-lookup"><span data-stu-id="3af3a-134">double</span></span> | <span data-ttu-id="3af3a-135">ビデオのフレーム レート。</span><span class="sxs-lookup"><span data-stu-id="3af3a-135">Frame rate of the video.</span></span>
| <span data-ttu-id="3af3a-136">**height**</span><span class="sxs-lookup"><span data-stu-id="3af3a-136">**height**</span></span>                | <span data-ttu-id="3af3a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3af3a-137">Int32</span></span>  | <span data-ttu-id="3af3a-138">ビデオの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="3af3a-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="3af3a-139">**width**</span><span class="sxs-lookup"><span data-stu-id="3af3a-139">**width**</span></span>                 | <span data-ttu-id="3af3a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3af3a-140">Int32</span></span>  | <span data-ttu-id="3af3a-141">ビデオの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="3af3a-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="3af3a-142">注釈</span><span class="sxs-lookup"><span data-stu-id="3af3a-142">Remarks</span></span>

<span data-ttu-id="3af3a-143">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3af3a-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
