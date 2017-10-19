---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: dd6ece46ce54fe791c0e6b5801287e2abad4fe48
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="video-resource-type"></a>Video リソース型

**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。

[**DriveItem**](driveitem.md) に null でない **video** ファセットがある場合、そのアイテムはビデオ ファイルを表します。
**Video** リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

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

## <a name="properties"></a>プロパティ

| プロパティ名             | 種類   | 説明
|:--------------------------|:-------|:----------------------------------------
| **audioBitsPerSample**    | Int32  | 1 サンプルあたりのオーディオ ビット数。
| **audioChannels**         | Int32  | オーディオ チャンネル数。
| **audioFormat**           | string | オーディオ形式の名前 (AAC、MP3 など)。
| **audioSamplesPerSecond** | Int32  | 1 秒あたりのオーディオ サンプル数。
| **bitrate**               | Int32  | 1 秒あたりのビデオのビット レート (ビット単位)。
| **duration**              | Int64  | ファイルの長さ (ミリ秒単位)。
| **fourCC**                | string | ビデオ形式の「4 文字コード」名。
| **framerate**             | double | ビデオのフレーム レート。
| **height**                | Int32  | ビデオの高さ (ピクセル単位)。
| **width**                 | Int32  | ビデオの幅 (ピクセル単位)。

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>注釈

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
