---
author: VinodRavichandran
ms.date: 09/10/2017
title: オーディオ
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4ff9e98b3024184298da144f90665ba2f192fef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535593"
---
# <a name="audio-facet"></a><span data-ttu-id="691ea-102">Audio ファセット</span><span class="sxs-lookup"><span data-stu-id="691ea-102">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="691ea-103">**オーディオ** リソースは、アイテムのオーディオ関連のプロパティを単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="691ea-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="691ea-p101">[**DriveItem**](driveitem.md) に null 以外の**オーディオ** ファセットがある場合、そのアイテムはオーディオ ファイルを表します。**オーディオ** リソースのプロパティは、ファイルからメタデータを抽出することで設定されます。</span><span class="sxs-lookup"><span data-stu-id="691ea-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="691ea-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="691ea-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="691ea-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="691ea-107">Properties</span></span>

| <span data-ttu-id="691ea-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="691ea-108">Property name</span></span>         | <span data-ttu-id="691ea-109">種類</span><span class="sxs-lookup"><span data-stu-id="691ea-109">Type</span></span>    | <span data-ttu-id="691ea-110">説明</span><span class="sxs-lookup"><span data-stu-id="691ea-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="691ea-111">**album**</span><span class="sxs-lookup"><span data-stu-id="691ea-111">**album**</span></span>             | <span data-ttu-id="691ea-112">string</span><span class="sxs-lookup"><span data-stu-id="691ea-112">string</span></span>  | <span data-ttu-id="691ea-113">このオーディオ ファイルのアルバムのタイトル。</span><span class="sxs-lookup"><span data-stu-id="691ea-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="691ea-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="691ea-114">**albumArtist**</span></span>       | <span data-ttu-id="691ea-115">string</span><span class="sxs-lookup"><span data-stu-id="691ea-115">string</span></span>  | <span data-ttu-id="691ea-116">オーディオ ファイルのアルバムに付けられたアーチスト名。</span><span class="sxs-lookup"><span data-stu-id="691ea-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="691ea-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="691ea-117">**artist**</span></span>            | <span data-ttu-id="691ea-118">string</span><span class="sxs-lookup"><span data-stu-id="691ea-118">string</span></span>  | <span data-ttu-id="691ea-119">オーディオ ファイルの歌手や奏者。</span><span class="sxs-lookup"><span data-stu-id="691ea-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="691ea-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="691ea-120">**bitrate**</span></span>           | <span data-ttu-id="691ea-121">Int32</span><span class="sxs-lookup"><span data-stu-id="691ea-121">Int32</span></span>   | <span data-ttu-id="691ea-122">kbps 単位で表されるビットレート。</span><span class="sxs-lookup"><span data-stu-id="691ea-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="691ea-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="691ea-123">**composers**</span></span>         | <span data-ttu-id="691ea-124">string</span><span class="sxs-lookup"><span data-stu-id="691ea-124">string</span></span>  | <span data-ttu-id="691ea-125">オーディオ ファイルの作曲者の名前。</span><span class="sxs-lookup"><span data-stu-id="691ea-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="691ea-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="691ea-126">**copyright**</span></span>         | <span data-ttu-id="691ea-127">string</span><span class="sxs-lookup"><span data-stu-id="691ea-127">string</span></span>  | <span data-ttu-id="691ea-128">オーディオ ファイルの著作権情報。</span><span class="sxs-lookup"><span data-stu-id="691ea-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="691ea-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="691ea-129">**disc**</span></span>              | <span data-ttu-id="691ea-130">Int32</span><span class="sxs-lookup"><span data-stu-id="691ea-130">Int32</span></span>   | <span data-ttu-id="691ea-131">このオーディオ ファイルの元のディスクの番号。</span><span class="sxs-lookup"><span data-stu-id="691ea-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="691ea-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="691ea-132">**discCount**</span></span>         | <span data-ttu-id="691ea-133">Int32</span><span class="sxs-lookup"><span data-stu-id="691ea-133">Int32</span></span>   | <span data-ttu-id="691ea-134">このアルバムの合計ディスク数。</span><span class="sxs-lookup"><span data-stu-id="691ea-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="691ea-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="691ea-135">**duration**</span></span>          | <span data-ttu-id="691ea-136">Int64</span><span class="sxs-lookup"><span data-stu-id="691ea-136">Int64</span></span>   | <span data-ttu-id="691ea-137">オーディオ ファイルの継続時間。ミリ秒単位で表されます。</span><span class="sxs-lookup"><span data-stu-id="691ea-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="691ea-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="691ea-138">**genre**</span></span>             | <span data-ttu-id="691ea-139">string</span><span class="sxs-lookup"><span data-stu-id="691ea-139">string</span></span>  | <span data-ttu-id="691ea-140">このオーディオ ファイルのジャンル。</span><span class="sxs-lookup"><span data-stu-id="691ea-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="691ea-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="691ea-141">**hasDrm**</span></span>            | <span data-ttu-id="691ea-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="691ea-142">boolean</span></span> | <span data-ttu-id="691ea-143">ファイルがデジタル著作権管理で保護されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="691ea-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="691ea-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="691ea-144">**isVariableBitrate**</span></span> | <span data-ttu-id="691ea-145">boolean</span><span class="sxs-lookup"><span data-stu-id="691ea-145">boolean</span></span> | <span data-ttu-id="691ea-146">ファイルが可変ビットレートでエンコードされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="691ea-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="691ea-147">**title**</span><span class="sxs-lookup"><span data-stu-id="691ea-147">**title**</span></span>             | <span data-ttu-id="691ea-148">string</span><span class="sxs-lookup"><span data-stu-id="691ea-148">string</span></span>  | <span data-ttu-id="691ea-149">オーディオ ファイルのタイトル。</span><span class="sxs-lookup"><span data-stu-id="691ea-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="691ea-150">**track**</span><span class="sxs-lookup"><span data-stu-id="691ea-150">**track**</span></span>             | <span data-ttu-id="691ea-151">Int32</span><span class="sxs-lookup"><span data-stu-id="691ea-151">Int32</span></span>   | <span data-ttu-id="691ea-152">このオーディオ ファイルの元のディスクでのトラック番号。</span><span class="sxs-lookup"><span data-stu-id="691ea-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="691ea-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="691ea-153">**trackCount**</span></span>        | <span data-ttu-id="691ea-154">Int32</span><span class="sxs-lookup"><span data-stu-id="691ea-154">Int32</span></span>   | <span data-ttu-id="691ea-155">このオーディオ ファイルの元のディスクの合計トラック数。</span><span class="sxs-lookup"><span data-stu-id="691ea-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="691ea-156">**year**</span><span class="sxs-lookup"><span data-stu-id="691ea-156">**year**</span></span>              | <span data-ttu-id="691ea-157">Int32</span><span class="sxs-lookup"><span data-stu-id="691ea-157">Int32</span></span>   | <span data-ttu-id="691ea-158">オーディオ ファイルが録音された年。</span><span class="sxs-lookup"><span data-stu-id="691ea-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="691ea-159">備考</span><span class="sxs-lookup"><span data-stu-id="691ea-159">Remarks</span></span>

<span data-ttu-id="691ea-160">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="691ea-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
