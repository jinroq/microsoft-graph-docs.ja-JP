---
title: room リソースの種類
description: テナント内のルームのプロパティを指定します。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 41c87daa31feda2907abab6f5711b4b88963095b
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841291"
---
# <a name="room-resource-type"></a>room リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナント内のルームを表します。 

Exchange Online では、各会議室が会議室メールボックスに関連付けられています。 派生元[](place.md)。

## <a name="methods"></a>メソッド

| メソッド                              | 戻り値の型                  | 説明 |
|:------------------------------------|:-----------------------------|:--------|
| [プレースを一覧表示する](../api/place-list.md) | 要求された派生型のコレクション。 [](place.md) | テナントで定義されている、指定された種類の**プレース**オブジェクトのコレクションを取得します。 たとえば、すべてのルーム、すべての会議室の一覧、または、テナント内の特定の会議室一覧の会議室を取得できます。 |
| [場所を取得する](../api/place-get.md)    | 要求された派生型[](place.md)            | ルームなど、指定された**place**オブジェクトのプロパティとリレーションシップを取得します。 |

## <a name="properties"></a>プロパティ

| プロパティ               | 型                                              | 説明 |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | 会議室の住所。 |
| audioDeviceName        | String                                            | ルーム内のオーディオデバイスの名前を指定します。 |
| bookingType            | [bookingType](#bookingtype-values)                | 部屋の種類。 可能な値は、`standard`、`managed`、`reserved` です。 |
| セキュリティ               | String                                            | 部屋がある建物名または建物番号を指定します。 |
| 最大               | String                                            | 会議室の容量を指定します。 |
| displayName            | String                                            | ルームに関連付けられた名前。 |
| displayDeviceName      | String                                            | ルームの表示デバイスの名前を指定します。 |
| emailAddress           | String                                            | 会議室の電子メールアドレス。 |
| floorNumber            | Int32                                             | 部屋があるフロア番号を指定します。 |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | 緯度、経度、および必要に応じて高度な座標での部屋の位置を指定します。 |
| id                     | 文字列                                            | ルームの一意識別子。 読み取り専用です。 |
| isWheelchairAccessible | Boolean                                           | 会議室に wheelchair アクセス可能かどうかを指定します。 |
| label                  | String                                            | ルームの内容を示すラベル (たとえば、数字または名前) を指定します。 |
| ニックネーム               | String                                            | 会議室のニックネームを指定します (例: "conf room")。 |
| phone                  | String                                            | 会議室の電話番号。 |
| タグ                   | String collection                                 | ルームの追加機能を指定します。たとえば、ビューや家具の種類などの詳細が表示されます。 |
| videoDeviceName        | String                                            | ルーム内のビデオデバイスの名前を指定します。 |

### <a name="bookingtype-values"></a>bookingType の値

| 値    | 説明                                               |
|:---------|:----------------------------------------------------------|
| standard | このコマンドレットの他の設定に基づいて、会議室を予約することができます。 所有者、作成者、サイト所有者は引き続き対象アイテムにアクセスできます。 |
| 対象  | 会議室が代理人によって管理されている                         |
| 予約語 | ルームは、最初に提供された最初の提供元でのみ利用可能です。 予約することはできません。|

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "String",
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelchairAccessible": true,
  "label": "String",
  "nickname": "String",
  "phone": "String",
  "tags": ["String"],
  "videoDeviceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "room resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
