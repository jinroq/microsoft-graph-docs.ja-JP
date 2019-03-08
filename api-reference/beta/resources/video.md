---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ビデオ
localization_priority: Normal
ms.openlocfilehash: 1e780c8392316be1f7fcc59f3818085dc462da29
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481595"
---
# <a name="video-resource-type"></a><span data-ttu-id="8b5f9-102">ビデオ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b5f9-102">Video resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b5f9-103">**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="8b5f9-p101">[**DriveItem**](driveitem.md) に null 以外の**ビデオ** ファセットがある場合は、項目はビデオ ファイルを表します。**ビデオ** リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b5f9-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b5f9-106">JSON representation</span></span>

<span data-ttu-id="8b5f9-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8b5f9-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="8b5f9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b5f9-108">Properties</span></span>

| <span data-ttu-id="8b5f9-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8b5f9-109">Property name</span></span>             | <span data-ttu-id="8b5f9-110">種類</span><span class="sxs-lookup"><span data-stu-id="8b5f9-110">Type</span></span>   | <span data-ttu-id="8b5f9-111">説明</span><span class="sxs-lookup"><span data-stu-id="8b5f9-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="8b5f9-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="8b5f9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8b5f9-113">Int32</span></span>  | <span data-ttu-id="8b5f9-114">サンプルあたりのオーディオ ビット数。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="8b5f9-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-115">**audioChannels**</span></span>         | <span data-ttu-id="8b5f9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8b5f9-116">Int32</span></span>  | <span data-ttu-id="8b5f9-117">オーディオ チャンネル数。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-117">Number of audio channels.</span></span>
| <span data-ttu-id="8b5f9-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-118">**audioFormat**</span></span>           | <span data-ttu-id="8b5f9-119">string</span><span class="sxs-lookup"><span data-stu-id="8b5f9-119">string</span></span> | <span data-ttu-id="8b5f9-120">オーディオ形式の名前 (AAC、MP3 など)。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="8b5f9-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="8b5f9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8b5f9-122">Int32</span></span>  | <span data-ttu-id="8b5f9-123">1 秒あたりのオーディオ サンプル数。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="8b5f9-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-124">**bitrate**</span></span>               | <span data-ttu-id="8b5f9-125">Int32</span><span class="sxs-lookup"><span data-stu-id="8b5f9-125">Int32</span></span>  | <span data-ttu-id="8b5f9-126">1 秒あたりのビデオのビット レート (ビット単位)。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="8b5f9-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-127">**duration**</span></span>              | <span data-ttu-id="8b5f9-128">Int64</span><span class="sxs-lookup"><span data-stu-id="8b5f9-128">Int64</span></span>  | <span data-ttu-id="8b5f9-129">ファイルの継続時間 (ミリ秒単位)。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="8b5f9-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-130">**fourCC**</span></span>                | <span data-ttu-id="8b5f9-131">string</span><span class="sxs-lookup"><span data-stu-id="8b5f9-131">string</span></span> | <span data-ttu-id="8b5f9-132">ビデオ形式の「4 文字コード」名。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="8b5f9-133">**framerate**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-133">**framerate**</span></span>             | <span data-ttu-id="8b5f9-134">double</span><span class="sxs-lookup"><span data-stu-id="8b5f9-134">double</span></span> | <span data-ttu-id="8b5f9-135">ビデオのフレーム レート。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-135">Frame rate of the video.</span></span>
| <span data-ttu-id="8b5f9-136">**height**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-136">**height**</span></span>                | <span data-ttu-id="8b5f9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8b5f9-137">Int32</span></span>  | <span data-ttu-id="8b5f9-138">ビデオの高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="8b5f9-139">**width**</span><span class="sxs-lookup"><span data-stu-id="8b5f9-139">**width**</span></span>                 | <span data-ttu-id="8b5f9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8b5f9-140">Int32</span></span>  | <span data-ttu-id="8b5f9-141">ビデオの幅 (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="8b5f9-142">注釈</span><span class="sxs-lookup"><span data-stu-id="8b5f9-142">Remarks</span></span>

<span data-ttu-id="8b5f9-143">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b5f9-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





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
