---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: オーディオ
ms.openlocfilehash: e68b70565f0eccd7847fba2b8085661071a75ae7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266234"
---
# <a name="audio-facet"></a>Audio ファセット

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

| プロパティ名         | 型    | 説明                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| **アルバム**             | 文字列  | このオーディオ ファイルのアルバムのタイトル。                          |
| **albumArtist**       | 文字列  | オーディオ ファイルのアルバムに付けられたアーチスト名。                    |
| **アーティスト**            | 文字列  | オーディオ ファイルの歌手や奏者。                            |
| **ビットレート**           | Int64   | kbps 単位で表されるビットレート。                                           |
| **作曲家**         | 文字列  | オーディオ ファイルの作曲者の名前。                          |
| **著作権**         | 文字列  | オーディオ ファイルの著作権情報。                            |
| **ディスク**              | Int16   | このオーディオ ファイルの元のディスクの番号。                    |
| **discCount**         | Int16   | このアルバムの合計ディスク数。                             |
| **期間**          | Int64   | オーディオ ファイルの継続時間。ミリ秒単位で表されます。                |
| **ジャンル**             | 文字列  | このオーディオ ファイルのジャンル。                                        |
| **hasDrm**            | ブール値 | ファイルがデジタル著作権管理で保護されているかどうかを示します。   |
| **isVariableBitrate** | ブール値 | ファイルが可変ビットレートでエンコードされているかどうかを示します。            |
| **タイトル**             | 文字列  | オーディオ ファイルのタイトル。                                         |
| **トラック**             | Int32   | このオーディオ ファイルの元のディスクでのトラック番号。    |
| **trackCount**        | Int32   | このオーディオ ファイルの元のディスクの合計トラック数。 |
| **年**              | Int32   | オーディオ ファイルが録音された年。                                |

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
