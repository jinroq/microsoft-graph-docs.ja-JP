---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: a9bf228d814526d089fb102444e6952558b07e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073275"
---
# <a name="video-resource-type"></a><span data-ttu-id="30eba-102">ビデオ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30eba-102">Video resource type</span></span>

> <span data-ttu-id="30eba-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30eba-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30eba-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30eba-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30eba-105">**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="30eba-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="30eba-p102">[**DriveItem**](driveitem.md) に null 以外の**ビデオ** ファセットがある場合は、項目はビデオ ファイルを表します。**ビデオ** リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。</span><span class="sxs-lookup"><span data-stu-id="30eba-p102">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30eba-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30eba-108">JSON representation</span></span>

<span data-ttu-id="30eba-109">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="30eba-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="30eba-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30eba-110">Properties</span></span>

| <span data-ttu-id="30eba-111">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="30eba-111">Property name</span></span>             | <span data-ttu-id="30eba-112">型</span><span class="sxs-lookup"><span data-stu-id="30eba-112">Type</span></span>   | <span data-ttu-id="30eba-113">説明</span><span class="sxs-lookup"><span data-stu-id="30eba-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="30eba-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="30eba-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="30eba-115">Int32</span><span class="sxs-lookup"><span data-stu-id="30eba-115">Int32</span></span>  | <span data-ttu-id="30eba-116">サンプルあたりのオーディオ ビット数。</span><span class="sxs-lookup"><span data-stu-id="30eba-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="30eba-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="30eba-117">**audioChannels**</span></span>         | <span data-ttu-id="30eba-118">Int32</span><span class="sxs-lookup"><span data-stu-id="30eba-118">Int32</span></span>  | <span data-ttu-id="30eba-119">オーディオ チャンネル数。</span><span class="sxs-lookup"><span data-stu-id="30eba-119">Number of audio channels.</span></span>
| <span data-ttu-id="30eba-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="30eba-120">**audioFormat**</span></span>           | <span data-ttu-id="30eba-121">文字列</span><span class="sxs-lookup"><span data-stu-id="30eba-121">string</span></span> | <span data-ttu-id="30eba-122">オーディオ形式の名前 (AAC、MP3 など)。</span><span class="sxs-lookup"><span data-stu-id="30eba-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="30eba-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="30eba-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="30eba-124">Int32</span><span class="sxs-lookup"><span data-stu-id="30eba-124">Int32</span></span>  | <span data-ttu-id="30eba-125">1 秒あたりのオーディオ サンプル数。</span><span class="sxs-lookup"><span data-stu-id="30eba-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="30eba-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="30eba-126">**bitrate**</span></span>               | <span data-ttu-id="30eba-127">Int32</span><span class="sxs-lookup"><span data-stu-id="30eba-127">Int32</span></span>  | <span data-ttu-id="30eba-128">1 秒あたりのビデオのビット レート (ビット単位)。</span><span class="sxs-lookup"><span data-stu-id="30eba-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="30eba-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="30eba-129">**duration**</span></span>              | <span data-ttu-id="30eba-130">Int64</span><span class="sxs-lookup"><span data-stu-id="30eba-130">Int64</span></span>  | <span data-ttu-id="30eba-131">ファイルの継続時間 (ミリ秒単位)。</span><span class="sxs-lookup"><span data-stu-id="30eba-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="30eba-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="30eba-132">**fourCC**</span></span>                | <span data-ttu-id="30eba-133">文字列</span><span class="sxs-lookup"><span data-stu-id="30eba-133">string</span></span> | <span data-ttu-id="30eba-134">ビデオ形式の「4 文字コード」名。</span><span class="sxs-lookup"><span data-stu-id="30eba-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="30eba-135">**framerate**</span><span class="sxs-lookup"><span data-stu-id="30eba-135">**framerate**</span></span>             | <span data-ttu-id="30eba-136">double</span><span class="sxs-lookup"><span data-stu-id="30eba-136">double</span></span> | <span data-ttu-id="30eba-137">ビデオのフレーム レート。</span><span class="sxs-lookup"><span data-stu-id="30eba-137">Frame rate of the video.</span></span>
| <span data-ttu-id="30eba-138">**height**</span><span class="sxs-lookup"><span data-stu-id="30eba-138">**height**</span></span>                | <span data-ttu-id="30eba-139">Int32</span><span class="sxs-lookup"><span data-stu-id="30eba-139">Int32</span></span>  | <span data-ttu-id="30eba-140">ビデオの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="30eba-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="30eba-141">**width**</span><span class="sxs-lookup"><span data-stu-id="30eba-141">**width**</span></span>                 | <span data-ttu-id="30eba-142">Int32</span><span class="sxs-lookup"><span data-stu-id="30eba-142">Int32</span></span>  | <span data-ttu-id="30eba-143">ビデオの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="30eba-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="30eba-144">注釈</span><span class="sxs-lookup"><span data-stu-id="30eba-144">Remarks</span></span>

<span data-ttu-id="30eba-145">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30eba-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": ""
}-->
