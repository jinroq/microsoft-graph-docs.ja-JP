---
author: VinodRavichandran
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd1f1af0e1ddcd1d56853c708da7ba03be740812
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573635"
---
# <a name="audio-facet"></a><span data-ttu-id="65837-102">Audio ファセット</span><span class="sxs-lookup"><span data-stu-id="65837-102">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65837-103">**オーディオ** リソースは、アイテムのオーディオ関連のプロパティを単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="65837-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="65837-p101">[**DriveItem**](driveitem.md) に null 以外の**オーディオ** ファセットがある場合、そのアイテムはオーディオ ファイルを表します。**オーディオ** リソースのプロパティは、ファイルからメタデータを抽出することで設定されます。</span><span class="sxs-lookup"><span data-stu-id="65837-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="65837-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65837-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="65837-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65837-107">Properties</span></span>

| <span data-ttu-id="65837-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="65837-108">Property name</span></span>         | <span data-ttu-id="65837-109">種類</span><span class="sxs-lookup"><span data-stu-id="65837-109">Type</span></span>    | <span data-ttu-id="65837-110">説明</span><span class="sxs-lookup"><span data-stu-id="65837-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="65837-111">**album**</span><span class="sxs-lookup"><span data-stu-id="65837-111">**album**</span></span>             | <span data-ttu-id="65837-112">string</span><span class="sxs-lookup"><span data-stu-id="65837-112">string</span></span>  | <span data-ttu-id="65837-113">このオーディオ ファイルのアルバムのタイトル。</span><span class="sxs-lookup"><span data-stu-id="65837-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="65837-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="65837-114">**albumArtist**</span></span>       | <span data-ttu-id="65837-115">string</span><span class="sxs-lookup"><span data-stu-id="65837-115">string</span></span>  | <span data-ttu-id="65837-116">オーディオ ファイルのアルバムに付けられたアーチスト名。</span><span class="sxs-lookup"><span data-stu-id="65837-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="65837-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="65837-117">**artist**</span></span>            | <span data-ttu-id="65837-118">string</span><span class="sxs-lookup"><span data-stu-id="65837-118">string</span></span>  | <span data-ttu-id="65837-119">オーディオ ファイルの歌手や奏者。</span><span class="sxs-lookup"><span data-stu-id="65837-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="65837-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="65837-120">**bitrate**</span></span>           | <span data-ttu-id="65837-121">Int64</span><span class="sxs-lookup"><span data-stu-id="65837-121">Int64</span></span>   | <span data-ttu-id="65837-122">kbps 単位で表されるビットレート。</span><span class="sxs-lookup"><span data-stu-id="65837-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="65837-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="65837-123">**composers**</span></span>         | <span data-ttu-id="65837-124">string</span><span class="sxs-lookup"><span data-stu-id="65837-124">string</span></span>  | <span data-ttu-id="65837-125">オーディオ ファイルの作曲者の名前。</span><span class="sxs-lookup"><span data-stu-id="65837-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="65837-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="65837-126">**copyright**</span></span>         | <span data-ttu-id="65837-127">string</span><span class="sxs-lookup"><span data-stu-id="65837-127">string</span></span>  | <span data-ttu-id="65837-128">オーディオ ファイルの著作権情報。</span><span class="sxs-lookup"><span data-stu-id="65837-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="65837-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="65837-129">**disc**</span></span>              | <span data-ttu-id="65837-130">Int16 型</span><span class="sxs-lookup"><span data-stu-id="65837-130">Int16</span></span>   | <span data-ttu-id="65837-131">このオーディオ ファイルの元のディスクの番号。</span><span class="sxs-lookup"><span data-stu-id="65837-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="65837-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="65837-132">**discCount**</span></span>         | <span data-ttu-id="65837-133">Int16 型</span><span class="sxs-lookup"><span data-stu-id="65837-133">Int16</span></span>   | <span data-ttu-id="65837-134">このアルバムの合計ディスク数。</span><span class="sxs-lookup"><span data-stu-id="65837-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="65837-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="65837-135">**duration**</span></span>          | <span data-ttu-id="65837-136">Int64</span><span class="sxs-lookup"><span data-stu-id="65837-136">Int64</span></span>   | <span data-ttu-id="65837-137">オーディオ ファイルの継続時間。ミリ秒単位で表されます。</span><span class="sxs-lookup"><span data-stu-id="65837-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="65837-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="65837-138">**genre**</span></span>             | <span data-ttu-id="65837-139">string</span><span class="sxs-lookup"><span data-stu-id="65837-139">string</span></span>  | <span data-ttu-id="65837-140">このオーディオ ファイルのジャンル。</span><span class="sxs-lookup"><span data-stu-id="65837-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="65837-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="65837-141">**hasDrm**</span></span>            | <span data-ttu-id="65837-142">boolean</span><span class="sxs-lookup"><span data-stu-id="65837-142">boolean</span></span> | <span data-ttu-id="65837-143">ファイルがデジタル著作権管理で保護されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65837-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="65837-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="65837-144">**isVariableBitrate**</span></span> | <span data-ttu-id="65837-145">boolean</span><span class="sxs-lookup"><span data-stu-id="65837-145">boolean</span></span> | <span data-ttu-id="65837-146">ファイルが可変ビットレートでエンコードされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="65837-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="65837-147">**title**</span><span class="sxs-lookup"><span data-stu-id="65837-147">**title**</span></span>             | <span data-ttu-id="65837-148">string</span><span class="sxs-lookup"><span data-stu-id="65837-148">string</span></span>  | <span data-ttu-id="65837-149">オーディオ ファイルのタイトル。</span><span class="sxs-lookup"><span data-stu-id="65837-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="65837-150">**track**</span><span class="sxs-lookup"><span data-stu-id="65837-150">**track**</span></span>             | <span data-ttu-id="65837-151">Int32</span><span class="sxs-lookup"><span data-stu-id="65837-151">Int32</span></span>   | <span data-ttu-id="65837-152">このオーディオ ファイルの元のディスクでのトラック番号。</span><span class="sxs-lookup"><span data-stu-id="65837-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="65837-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="65837-153">**trackCount**</span></span>        | <span data-ttu-id="65837-154">Int32</span><span class="sxs-lookup"><span data-stu-id="65837-154">Int32</span></span>   | <span data-ttu-id="65837-155">このオーディオ ファイルの元のディスクの合計トラック数。</span><span class="sxs-lookup"><span data-stu-id="65837-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="65837-156">**year**</span><span class="sxs-lookup"><span data-stu-id="65837-156">**year**</span></span>              | <span data-ttu-id="65837-157">Int32</span><span class="sxs-lookup"><span data-stu-id="65837-157">Int32</span></span>   | <span data-ttu-id="65837-158">オーディオ ファイルが録音された年。</span><span class="sxs-lookup"><span data-stu-id="65837-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="65837-159">備考</span><span class="sxs-lookup"><span data-stu-id="65837-159">Remarks</span></span>

<span data-ttu-id="65837-160">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65837-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": [
    "Error: /api-reference/beta/resources/audio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
