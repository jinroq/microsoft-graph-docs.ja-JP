---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ビデオ
localization_priority: Normal
description: ビデオ リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 24af35fff4e867caa8e7052c821cb44d1f2c3755
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033433"
---
# <a name="video-resource-type"></a>ビデオ リソースの種類

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

| プロパティ名             | 種類   | 説明
|:--------------------------|:-------|:----------------------------------------
| **audioBitsPerSample**    | Int32  | サンプルあたりのオーディオ ビット数。
| **audioChannels**         | Int32  | オーディオ チャンネル数。
| **audioFormat**           | string | オーディオ形式の名前 (AAC、MP3 など)。
| **audioSamplesPerSecond** | Int32  | 1 秒あたりのオーディオ サンプル数。
| **bitrate**               | Int32  | 1 秒あたりのビデオのビット レート (ビット単位)。
| **duration**              | Int64  | ファイルの継続時間 (ミリ秒単位)。
| **fourCC**                | string | ビデオ形式の「4 文字コード」名。
| **frameRate**             | double | ビデオのフレーム レート。
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
