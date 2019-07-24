---
title: roomList リソースの種類
description: 会社によって作成されたルームのグループを表します。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f0c56f986663c71d8c6817c0024919e8714af94a
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841256"
---
# <a name="roomlist-resource-type"></a>roomList リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントで定義されている[ルーム](room.md)オブジェクトのグループを表します。

派生元[](place.md)。

## <a name="methods"></a>メソッド

| メソッド                              | 戻り値の型                  | 説明 |
|:------------------------------------|:-----------------------------|:--------|
| [プレースを一覧表示する](../api/place-list.md) | 要求された派生型のコレクション。 [](place.md) | テナントで定義されている、指定された種類の**プレース**オブジェクトのコレクションを取得します。 たとえば、すべてのルーム、すべての会議室の一覧、または、テナント内の特定の会議室一覧の会議室を取得できます。|
| [場所を取得する](../api/place-get.md)    | 要求された派生型[](place.md)            | ルームリストなど、指定した**place**オブジェクトのプロパティとリレーションシップを取得します。 |

## <a name="properties"></a>プロパティ

| プロパティ       | 型                                              | 説明 |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | 会議室リストの住所。 |
| displayName    | String                                            | 会議室一覧に関連付けられた名前。 |
| emailAddress   | String                                            | 会議室一覧の電子メールアドレス。 |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 緯度、経度、および (オプションで) 高度座標での roomlist の位置を指定します。 |
| id             | 文字列                                            | 会議室一覧の一意の識別子。 読み取り専用です。 |
| phone          | String                                            | 会議室一覧の電話番号。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                         | 説明          |
|:-------------|:-----------------------------|:---------------------|
| ルーム        | コレクションを[配置](place.md)する | 読み取り専用。Null 許容型です。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roomList"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "emailAddress": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "phone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roomList resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
