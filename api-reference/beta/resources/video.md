---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
localization_priority: Normal
ms.openlocfilehash: db560abc31daecc6064820ef6ef958808ddbc297
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508546"
---
# <a name="video-resource-type"></a><span data-ttu-id="bc30e-102">ビデオ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc30e-102">Video resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc30e-103">**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="bc30e-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="bc30e-p101">DriveItem に null 以外のビデオ ファセットがある場合は、項目はビデオ ファイルを表します。ビデオ リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。</span><span class="sxs-lookup"><span data-stu-id="bc30e-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc30e-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc30e-106">JSON representation</span></span>

<span data-ttu-id="bc30e-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="bc30e-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="bc30e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc30e-108">Properties</span></span>

| <span data-ttu-id="bc30e-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="bc30e-109">Property name</span></span>             | <span data-ttu-id="bc30e-110">種類</span><span class="sxs-lookup"><span data-stu-id="bc30e-110">Type</span></span>   | <span data-ttu-id="bc30e-111">説明</span><span class="sxs-lookup"><span data-stu-id="bc30e-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="bc30e-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="bc30e-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="bc30e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bc30e-113">Int32</span></span>  | <span data-ttu-id="bc30e-114">サンプルあたりのオーディオ ビット数。</span><span class="sxs-lookup"><span data-stu-id="bc30e-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="bc30e-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="bc30e-115">**audioChannels**</span></span>         | <span data-ttu-id="bc30e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bc30e-116">Int32</span></span>  | <span data-ttu-id="bc30e-117">オーディオ チャンネル数。</span><span class="sxs-lookup"><span data-stu-id="bc30e-117">Number of audio channels.</span></span>
| <span data-ttu-id="bc30e-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="bc30e-118">**audioFormat**</span></span>           | <span data-ttu-id="bc30e-119">string</span><span class="sxs-lookup"><span data-stu-id="bc30e-119">string</span></span> | <span data-ttu-id="bc30e-120">オーディオ形式の名前 (AAC、MP3 など)。</span><span class="sxs-lookup"><span data-stu-id="bc30e-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="bc30e-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="bc30e-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="bc30e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="bc30e-122">Int32</span></span>  | <span data-ttu-id="bc30e-123">1 秒あたりのオーディオ サンプル数。</span><span class="sxs-lookup"><span data-stu-id="bc30e-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="bc30e-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="bc30e-124">**bitrate**</span></span>               | <span data-ttu-id="bc30e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bc30e-125">Int32</span></span>  | <span data-ttu-id="bc30e-126">1 秒あたりのビデオのビット レート (ビット単位)。</span><span class="sxs-lookup"><span data-stu-id="bc30e-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="bc30e-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="bc30e-127">**duration**</span></span>              | <span data-ttu-id="bc30e-128">Int64</span><span class="sxs-lookup"><span data-stu-id="bc30e-128">Int64</span></span>  | <span data-ttu-id="bc30e-129">ファイルの継続時間 (ミリ秒単位)。</span><span class="sxs-lookup"><span data-stu-id="bc30e-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="bc30e-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="bc30e-130">**fourCC**</span></span>                | <span data-ttu-id="bc30e-131">string</span><span class="sxs-lookup"><span data-stu-id="bc30e-131">string</span></span> | <span data-ttu-id="bc30e-132">ビデオ形式の「4 文字コード」名。</span><span class="sxs-lookup"><span data-stu-id="bc30e-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="bc30e-133">**framerate**</span><span class="sxs-lookup"><span data-stu-id="bc30e-133">**framerate**</span></span>             | <span data-ttu-id="bc30e-134">double</span><span class="sxs-lookup"><span data-stu-id="bc30e-134">double</span></span> | <span data-ttu-id="bc30e-135">ビデオのフレーム レート。</span><span class="sxs-lookup"><span data-stu-id="bc30e-135">Frame rate of the video.</span></span>
| <span data-ttu-id="bc30e-136">**height**</span><span class="sxs-lookup"><span data-stu-id="bc30e-136">**height**</span></span>                | <span data-ttu-id="bc30e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bc30e-137">Int32</span></span>  | <span data-ttu-id="bc30e-138">ビデオの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="bc30e-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="bc30e-139">**width**</span><span class="sxs-lookup"><span data-stu-id="bc30e-139">**width**</span></span>                 | <span data-ttu-id="bc30e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bc30e-140">Int32</span></span>  | <span data-ttu-id="bc30e-141">ビデオの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="bc30e-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="bc30e-142">注釈</span><span class="sxs-lookup"><span data-stu-id="bc30e-142">Remarks</span></span>

<span data-ttu-id="bc30e-143">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc30e-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/video.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
