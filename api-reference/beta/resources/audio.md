---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
ms.openlocfilehash: 1472bffec12ed5626a65ea71b971dc5bc2b77aa9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068411"
---
# <a name="audio-facet"></a><span data-ttu-id="2b2bc-102">Audio ファセット</span><span class="sxs-lookup"><span data-stu-id="2b2bc-102">Audio facet</span></span>

> <span data-ttu-id="2b2bc-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b2bc-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b2bc-105">**オーディオ** リソースは、アイテムのオーディオ関連のプロパティを単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="2b2bc-p102">[**DriveItem**](driveitem.md) に null 以外の**オーディオ** ファセットがある場合、そのアイテムはオーディオ ファイルを表します。**オーディオ** リソースのプロパティは、ファイルからメタデータを抽出することで設定されます。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-p102">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="2b2bc-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b2bc-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2b2bc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b2bc-109">Properties</span></span>

| <span data-ttu-id="2b2bc-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2b2bc-110">Property name</span></span>         | <span data-ttu-id="2b2bc-111">型</span><span class="sxs-lookup"><span data-stu-id="2b2bc-111">Type</span></span>    | <span data-ttu-id="2b2bc-112">説明</span><span class="sxs-lookup"><span data-stu-id="2b2bc-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="2b2bc-113">**album**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-113">**album**</span></span>             | <span data-ttu-id="2b2bc-114">文字列</span><span class="sxs-lookup"><span data-stu-id="2b2bc-114">string</span></span>  | <span data-ttu-id="2b2bc-115">このオーディオ ファイルのアルバムのタイトル。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="2b2bc-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-116">**albumArtist**</span></span>       | <span data-ttu-id="2b2bc-117">文字列</span><span class="sxs-lookup"><span data-stu-id="2b2bc-117">string</span></span>  | <span data-ttu-id="2b2bc-118">オーディオ ファイルのアルバムに付けられたアーチスト名。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="2b2bc-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-119">**artist**</span></span>            | <span data-ttu-id="2b2bc-120">文字列</span><span class="sxs-lookup"><span data-stu-id="2b2bc-120">string</span></span>  | <span data-ttu-id="2b2bc-121">オーディオ ファイルの歌手や奏者。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="2b2bc-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-122">**bitrate**</span></span>           | <span data-ttu-id="2b2bc-123">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2bc-123">Int32</span></span>   | <span data-ttu-id="2b2bc-124">kbps 単位で表されるビットレート。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="2b2bc-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-125">**composers**</span></span>         | <span data-ttu-id="2b2bc-126">文字列</span><span class="sxs-lookup"><span data-stu-id="2b2bc-126">string</span></span>  | <span data-ttu-id="2b2bc-127">オーディオ ファイルの作曲者の名前。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="2b2bc-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-128">**copyright**</span></span>         | <span data-ttu-id="2b2bc-129">文字列</span><span class="sxs-lookup"><span data-stu-id="2b2bc-129">string</span></span>  | <span data-ttu-id="2b2bc-130">オーディオ ファイルの著作権情報。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="2b2bc-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-131">**disc**</span></span>              | <span data-ttu-id="2b2bc-132">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2bc-132">Int32</span></span>   | <span data-ttu-id="2b2bc-133">このオーディオ ファイルの元のディスクの番号。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="2b2bc-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-134">**discCount**</span></span>         | <span data-ttu-id="2b2bc-135">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2bc-135">Int32</span></span>   | <span data-ttu-id="2b2bc-136">このアルバムの合計ディスク数。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="2b2bc-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-137">**duration**</span></span>          | <span data-ttu-id="2b2bc-138">Int64</span><span class="sxs-lookup"><span data-stu-id="2b2bc-138">Int64</span></span>   | <span data-ttu-id="2b2bc-139">オーディオ ファイルの継続時間。ミリ秒単位で表されます。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="2b2bc-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-140">**genre**</span></span>             | <span data-ttu-id="2b2bc-141">文字列</span><span class="sxs-lookup"><span data-stu-id="2b2bc-141">string</span></span>  | <span data-ttu-id="2b2bc-142">このオーディオ ファイルのジャンル。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="2b2bc-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-143">**hasDrm**</span></span>            | <span data-ttu-id="2b2bc-144">boolean</span><span class="sxs-lookup"><span data-stu-id="2b2bc-144">boolean</span></span> | <span data-ttu-id="2b2bc-145">ファイルがデジタル著作権管理で保護されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="2b2bc-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-146">**isVariableBitrate**</span></span> | <span data-ttu-id="2b2bc-147">boolean</span><span class="sxs-lookup"><span data-stu-id="2b2bc-147">boolean</span></span> | <span data-ttu-id="2b2bc-148">ファイルが可変ビットレートでエンコードされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="2b2bc-149">**title**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-149">**title**</span></span>             | <span data-ttu-id="2b2bc-150">文字列</span><span class="sxs-lookup"><span data-stu-id="2b2bc-150">string</span></span>  | <span data-ttu-id="2b2bc-151">オーディオ ファイルのタイトル。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="2b2bc-152">**track**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-152">**track**</span></span>             | <span data-ttu-id="2b2bc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2bc-153">Int32</span></span>   | <span data-ttu-id="2b2bc-154">このオーディオ ファイルの元のディスクでのトラック番号。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="2b2bc-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-155">**trackCount**</span></span>        | <span data-ttu-id="2b2bc-156">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2bc-156">Int32</span></span>   | <span data-ttu-id="2b2bc-157">このオーディオ ファイルの元のディスクの合計トラック数。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="2b2bc-158">**year**</span><span class="sxs-lookup"><span data-stu-id="2b2bc-158">**year**</span></span>              | <span data-ttu-id="2b2bc-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2bc-159">Int32</span></span>   | <span data-ttu-id="2b2bc-160">オーディオ ファイルが録音された年。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="2b2bc-161">備考</span><span class="sxs-lookup"><span data-stu-id="2b2bc-161">Remarks</span></span>

<span data-ttu-id="2b2bc-162">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b2bc-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
