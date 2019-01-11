---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
localization_priority: Normal
ms.openlocfilehash: 3883dd494304409b76d10781039424267ada85f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866634"
---
# <a name="video-resource-type"></a>ビデオ リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。

[**DriveItem**](driveitem.md) に null 以外の**ビデオ** ファセットがある場合は、項目はビデオ ファイルを表します。**ビデオ** リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。

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

| プロパティ名             | Type   | 説明
|:--------------------------|:-------|:----------------------------------------
| **audioBitsPerSample**    | Int32  | サンプルあたりのオーディオ ビット数。
| **audioChannels**         | Int32  | オーディオ チャンネル数。
| **audioFormat**           | 文字列 | オーディオ形式の名前 (AAC、MP3 など)。
| **audioSamplesPerSecond** | Int32  | 1 秒あたりのオーディオ サンプル数。
| **bitrate**               | Int32  | 1 秒あたりのビデオのビット レート (ビット単位)。
| **duration**              | Int64  | ファイルの継続時間 (ミリ秒単位)。
| **fourCC**                | 文字列 | ビデオ形式の「4 文字コード」名。
| **framerate**             | double | ビデオのフレーム レート。
| **height**                | Int32  | ビデオの高さ (ピクセル単位)。
| **width**                 | Int32  | ビデオの幅 (ピクセル単位)。

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>注釈

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": ""
}-->
