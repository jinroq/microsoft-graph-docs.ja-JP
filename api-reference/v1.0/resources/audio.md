---
author: VinodRavichandran
ms.date: 09/10/2017
title: オーディオ
localization_priority: Normal
ms.prod: microsoft-teams
description: オーディオ リソースは、アイテムのオーディオ関連のプロパティを単一の構造にグループ化します。
doc_type: resourcePageType
ms.openlocfilehash: a71b9ee9c65bacc802244bda2e7757e87d9ff35e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030024"
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

| プロパティ名         | 種類    | 説明                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| **album**             | string  | このオーディオ ファイルのアルバムのタイトル。                          |
| **albumArtist**       | string  | オーディオ ファイルのアルバムに付けられたアーチスト名。                    |
| **artist**            | string  | オーディオ ファイルの歌手や奏者。                            |
| **bitrate**           | Int64   | kbps 単位で表されるビットレート。                                           |
| **composers**         | string  | オーディオ ファイルの作曲者の名前。                          |
| **copyright**         | string  | オーディオ ファイルの著作権情報。                            |
| **disc**              | Int16   | このオーディオ ファイルの元のディスクの番号。                    |
| **discCount**         | Int16   | このアルバムの合計ディスク数。                             |
| **duration**          | Int64   | オーディオ ファイルの継続時間。ミリ秒単位で表されます。                |
| **genre**             | string  | このオーディオ ファイルのジャンル。                                        |
| **hasDrm**            | ブール値 | ファイルがデジタル著作権管理で保護されているかどうかを示します。   |
| **isVariableBitrate** | boolean | ファイルが可変ビットレートでエンコードされているかどうかを示します。            |
| **title**             | string  | オーディオ ファイルのタイトル。                                         |
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
