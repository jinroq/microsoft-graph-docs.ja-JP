---
author: VinodRavichandran
description: オーディオ リソースは、アイテムのオーディオ関連のプロパティを単一の構造にグループ化します。
ms.date: 09/10/2017
title: オーディオ
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 078ade2fd92d6eaf8d9017fe5cd8255a7449769e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013228"
---
# <a name="audio-facet"></a><span data-ttu-id="da87e-103">Audio ファセット</span><span class="sxs-lookup"><span data-stu-id="da87e-103">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da87e-104">**オーディオ** リソースは、アイテムのオーディオ関連のプロパティを単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="da87e-104">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="da87e-p101">[**DriveItem**](driveitem.md) に null 以外の**オーディオ** ファセットがある場合、そのアイテムはオーディオ ファイルを表します。**オーディオ** リソースのプロパティは、ファイルからメタデータを抽出することで設定されます。</span><span class="sxs-lookup"><span data-stu-id="da87e-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="da87e-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da87e-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a><span data-ttu-id="da87e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da87e-108">Properties</span></span>

| <span data-ttu-id="da87e-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="da87e-109">Property name</span></span>         | <span data-ttu-id="da87e-110">種類</span><span class="sxs-lookup"><span data-stu-id="da87e-110">Type</span></span>    | <span data-ttu-id="da87e-111">説明</span><span class="sxs-lookup"><span data-stu-id="da87e-111">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="da87e-112">**album**</span><span class="sxs-lookup"><span data-stu-id="da87e-112">**album**</span></span>             | <span data-ttu-id="da87e-113">string</span><span class="sxs-lookup"><span data-stu-id="da87e-113">string</span></span>  | <span data-ttu-id="da87e-114">このオーディオ ファイルのアルバムのタイトル。</span><span class="sxs-lookup"><span data-stu-id="da87e-114">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="da87e-115">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="da87e-115">**albumArtist**</span></span>       | <span data-ttu-id="da87e-116">string</span><span class="sxs-lookup"><span data-stu-id="da87e-116">string</span></span>  | <span data-ttu-id="da87e-117">オーディオ ファイルのアルバムに付けられたアーチスト名。</span><span class="sxs-lookup"><span data-stu-id="da87e-117">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="da87e-118">**artist**</span><span class="sxs-lookup"><span data-stu-id="da87e-118">**artist**</span></span>            | <span data-ttu-id="da87e-119">string</span><span class="sxs-lookup"><span data-stu-id="da87e-119">string</span></span>  | <span data-ttu-id="da87e-120">オーディオ ファイルの歌手や奏者。</span><span class="sxs-lookup"><span data-stu-id="da87e-120">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="da87e-121">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="da87e-121">**bitrate**</span></span>           | <span data-ttu-id="da87e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="da87e-122">Int32</span></span>   | <span data-ttu-id="da87e-123">kbps 単位で表されるビットレート。</span><span class="sxs-lookup"><span data-stu-id="da87e-123">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="da87e-124">**composers**</span><span class="sxs-lookup"><span data-stu-id="da87e-124">**composers**</span></span>         | <span data-ttu-id="da87e-125">string</span><span class="sxs-lookup"><span data-stu-id="da87e-125">string</span></span>  | <span data-ttu-id="da87e-126">オーディオ ファイルの作曲者の名前。</span><span class="sxs-lookup"><span data-stu-id="da87e-126">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="da87e-127">**copyright**</span><span class="sxs-lookup"><span data-stu-id="da87e-127">**copyright**</span></span>         | <span data-ttu-id="da87e-128">string</span><span class="sxs-lookup"><span data-stu-id="da87e-128">string</span></span>  | <span data-ttu-id="da87e-129">オーディオ ファイルの著作権情報。</span><span class="sxs-lookup"><span data-stu-id="da87e-129">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="da87e-130">**disc**</span><span class="sxs-lookup"><span data-stu-id="da87e-130">**disc**</span></span>              | <span data-ttu-id="da87e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="da87e-131">Int32</span></span>   | <span data-ttu-id="da87e-132">このオーディオ ファイルの元のディスクの番号。</span><span class="sxs-lookup"><span data-stu-id="da87e-132">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="da87e-133">**discCount**</span><span class="sxs-lookup"><span data-stu-id="da87e-133">**discCount**</span></span>         | <span data-ttu-id="da87e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="da87e-134">Int32</span></span>   | <span data-ttu-id="da87e-135">このアルバムの合計ディスク数。</span><span class="sxs-lookup"><span data-stu-id="da87e-135">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="da87e-136">**duration**</span><span class="sxs-lookup"><span data-stu-id="da87e-136">**duration**</span></span>          | <span data-ttu-id="da87e-137">Int64</span><span class="sxs-lookup"><span data-stu-id="da87e-137">Int64</span></span>   | <span data-ttu-id="da87e-138">オーディオ ファイルの継続時間。ミリ秒単位で表されます。</span><span class="sxs-lookup"><span data-stu-id="da87e-138">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="da87e-139">**genre**</span><span class="sxs-lookup"><span data-stu-id="da87e-139">**genre**</span></span>             | <span data-ttu-id="da87e-140">string</span><span class="sxs-lookup"><span data-stu-id="da87e-140">string</span></span>  | <span data-ttu-id="da87e-141">このオーディオ ファイルのジャンル。</span><span class="sxs-lookup"><span data-stu-id="da87e-141">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="da87e-142">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="da87e-142">**hasDrm**</span></span>            | <span data-ttu-id="da87e-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="da87e-143">boolean</span></span> | <span data-ttu-id="da87e-144">ファイルがデジタル著作権管理で保護されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da87e-144">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="da87e-145">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="da87e-145">**isVariableBitrate**</span></span> | <span data-ttu-id="da87e-146">boolean</span><span class="sxs-lookup"><span data-stu-id="da87e-146">boolean</span></span> | <span data-ttu-id="da87e-147">ファイルが可変ビットレートでエンコードされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da87e-147">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="da87e-148">**title**</span><span class="sxs-lookup"><span data-stu-id="da87e-148">**title**</span></span>             | <span data-ttu-id="da87e-149">string</span><span class="sxs-lookup"><span data-stu-id="da87e-149">string</span></span>  | <span data-ttu-id="da87e-150">オーディオ ファイルのタイトル。</span><span class="sxs-lookup"><span data-stu-id="da87e-150">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="da87e-151">**track**</span><span class="sxs-lookup"><span data-stu-id="da87e-151">**track**</span></span>             | <span data-ttu-id="da87e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="da87e-152">Int32</span></span>   | <span data-ttu-id="da87e-153">このオーディオ ファイルの元のディスクでのトラック番号。</span><span class="sxs-lookup"><span data-stu-id="da87e-153">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="da87e-154">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="da87e-154">**trackCount**</span></span>        | <span data-ttu-id="da87e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="da87e-155">Int32</span></span>   | <span data-ttu-id="da87e-156">このオーディオ ファイルの元のディスクの合計トラック数。</span><span class="sxs-lookup"><span data-stu-id="da87e-156">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="da87e-157">**year**</span><span class="sxs-lookup"><span data-stu-id="da87e-157">**year**</span></span>              | <span data-ttu-id="da87e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="da87e-158">Int32</span></span>   | <span data-ttu-id="da87e-159">オーディオ ファイルが録音された年。</span><span class="sxs-lookup"><span data-stu-id="da87e-159">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="da87e-160">備考</span><span class="sxs-lookup"><span data-stu-id="da87e-160">Remarks</span></span>

<span data-ttu-id="da87e-161">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da87e-161">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": []
}
-->
