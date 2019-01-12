---
author: VinodRavichandran
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b88fbbcd11a4cbeff56c870225d7b0bef4b32346
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985376"
---
# <a name="audio-facet"></a>Audio ファセット

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**オーディオ** リソースは、アイテムのオーディオ関連のプロパティを単一の構造にグループ化します。

[**DriveItem**](driveitem.md) に null 以外の**オーディオ** ファセットがある場合、そのアイテムはオーディオ ファイルを表します。**オーディオ** リソースのプロパティは、ファイルからメタデータを抽出することで設定されます。 

## <a name="json-representation"></a>JSON 表記

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

## <a name="properties"></a>プロパティ

| プロパティ名         | Type    | 説明                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| **album**             | 文字列  | このオーディオ ファイルのアルバムのタイトル。                          |
| **albumArtist**       | 文字列  | オーディオ ファイルのアルバムに付けられたアーチスト名。                    |
| **artist**            | 文字列  | オーディオ ファイルの歌手や奏者。                            |
| **bitrate**           | Int32   | kbps 単位で表されるビットレート。                                           |
| **composers**         | 文字列  | オーディオ ファイルの作曲者の名前。                          |
| **copyright**         | 文字列  | オーディオ ファイルの著作権情報。                            |
| **disc**              | Int32   | このオーディオ ファイルの元のディスクの番号。                    |
| **discCount**         | Int32   | このアルバムの合計ディスク数。                             |
| **duration**          | Int64   | オーディオ ファイルの継続時間。ミリ秒単位で表されます。                |
| **genre**             | 文字列  | このオーディオ ファイルのジャンル。                                        |
| **hasDrm**            | boolean | ファイルがデジタル著作権管理で保護されているかどうかを示します。   |
| **isVariableBitrate** | boolean | ファイルが可変ビットレートでエンコードされているかどうかを示します。            |
| **title**             | 文字列  | オーディオ ファイルのタイトル。                                         |
| **track**             | Int32   | このオーディオ ファイルの元のディスクでのトラック番号。    |
| **trackCount**        | Int32   | このオーディオ ファイルの元のディスクの合計トラック数。 |
| **year**              | Int32   | オーディオ ファイルが録音された年。                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>備考

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
