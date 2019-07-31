---
title: dateTimeTimeZone リソースの種類
description: 特定時点の日付、時刻、およびタイム ゾーンを記述します。
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 28f9956c065e59a0db1ffbd0b82175546d3e5139
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973121"
---
# <a name="datetimetimezone-resource-type"></a>dateTimeTimeZone リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定時点の日付、時刻、およびタイム ゾーンを記述します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|dateTime|String|特定時点の日付と時刻を組み合わせた表現 (`{date}T{time}`)。 たとえば、"2019-04-16T09:00:00" とします。|
|timeZone|String|タイムゾーン ("太平洋標準時" など) を表します。 指定可能な値については、以下を参照してください。|

通常、 **timeZone**プロパティは、 [Windows で現在サポートさ](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones)れている任意のタイムゾーン、および[予定表 API でサポートさ](#additional-time-zones)れている追加のタイムゾーンに設定_でき_ます。 

**DateTimeTimeZone**をメソッド (イベントの[作成](../api/user-post-events.md)や[更新](../api/event-update.md)など) と組み合わせて使用する場合は、サポートされている実際のタイムゾーンをメモする必要があります。これは小さなサブセットになることがあります。

### <a name="additional-time-zones"></a>追加のタイムゾーン

Etc/GMT+12

Etc/GMT+11

太平洋/ホノルル

アメリカ/アンカレッジ

アメリカ/サンタイサベル

アメリカ/ロサンゼルス

アメリカ/フェニックス

アメリカ/チワワ

アメリカ/デンバー

アメリカ/グアテマラ

アメリカ/シカゴ

アメリカ/メキシコシティ

アメリカ/リジャイナ

アメリカ/ボゴタ

アメリカ/ニューヨーク

アメリカ/インディアナ/インディアナポリス

アメリカ/カラカス

アメリカ/アスンシオン

アメリカ/ハリファックス

アメリカ/クイアバ

アメリカ/ラパス

アメリカ/サンティアゴ

アメリカ/セントジョンズ

アメリカ/サンパウロ

アメリカ/アルゼンチン/ブエノスアイレス

アメリカ/カイエンヌ

アメリカ/ゴットホープ

アメリカ/モンテビデオ

アメリカ/バイア

Etc/GMT+2

大西洋/アゾレス諸島

大西洋/カーボベルデ

アフリカ/カサブランカ

Etc/GMT

ヨーロッパ/ロンドン

大西洋/レイキャビク

ヨーロッパ/ベルリン

ヨーロッパ/ブダペスト

ヨーロッパ/パリ

ヨーロッパ/ワルシャワ

アフリカ/ラゴス

アフリカ/ウィントフック

ヨーロッパ/ブカレスト

アジア/ベイルート

アフリカ/カイロ

アジア/ダマスカス

アフリカ/ヨハネスブルグ

ヨーロッパ/キエフ

ヨーロッパ/イスタンブール

アジア/エルサレム

アジア/アンマン

アジア/バグダッド

ヨーロッパ/カリーニングラード

アジア/リャド

アフリカ/ナイロビ

アジア/テヘラン

アジア/ドバイ

アジア/バクー

ヨーロッパ/モスクワ

インド/モーリシャス

アジア/トビリシ

アジア/エレバン

アジア/カブール

アジア/カラチ

アジア/タシケント

アジア/コルカタ

アジア/コロンボ

アジア/カトマンズ

アジア/アスタナ (アルマトイ)

アジア/ダッカ

アジア/エカテリンブルク

アジア/ヤンゴン (ラングーン)

アジア/バンコク

アジア/ノボシビルスク

アジア/上海

アジア/クラスノヤルスク

アジア/シンガポール

オーストラリア/パース

アジア/台北

アジア/ウランバートル

アジア/イルクーツク

アジア/東京

アジア/ソウル

オーストラリア/アデレード

オーストラリア/ダーウィン

オーストラリア/ブリスベン

オーストラリア/シドニー

太平洋/ポートモレスビー

オーストラリア/ホバート

アジア/ヤクーツク

太平洋/ガダルカナル島

アジア/ウラジオストク

太平洋/オークランド

Etc/GMT-12

太平洋/フィジー

アジア/マガダン

太平洋/トンガタプ

太平洋/アピア

太平洋/クリスマス島

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
