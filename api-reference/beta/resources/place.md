---
title: リソースの種類を配置する
description: 場所を表します。 これは、room または roomList の基本型です。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5cea04931d537c8b0bd29c49327a56afe8a7d5d5
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841298"
---
# <a name="place-resource-type"></a>リソースの種類を配置する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

名前、物理アドレス、地理的な座標などの基本的な場所の属性を表します。 これは、 [room](room.md)や[roomList](roomlist.md)などの豊富な場所の種類の基本型です。

### <a name="using-the-places-api"></a>プレース API の使用
Exchange Online 管理者は、テナント内の会議室を会議室一覧にまとめることができます。 プレース API を使用すると、テナント内のすべての会議室一覧またはルームを取得したり、特定の会議室一覧のすべての会議室を取得したりできます。

[Room](room.md)や[roomList](roomlist.md)などの場所には、基本**id**、表示名、電子メールアドレスが含まれています。 また、物理アドレスと地理的な座標、ルームの場合は、AV 能力、フロア番号、容量などの他の関連情報などのナビゲーション情報も含まれます。

[Findrooms](../api/user-findrooms.md)および[fin/omlists](../api/user-findroomlists.md)関数は、テナント内のルームおよび会議室一覧に類似した参照をサポートしています。 以下に、プレース API とこれらの関数の比較を示します。

|配置 API |Findrooms および fin/Omlists 関数|
|:------------------------------------|:-----------------------------|
|テナント内のすべての部屋または会議室一覧の取得、および会議室一覧のすべての会議室の取得をサポートしています。 | 同様のサポート-テナント内のすべてのルームまたはルームリストと、ルームリスト内のすべてのルームを取得します。|
|[リストの場所](../api/place-list.md)がテナント内の100ルームを超えることがある | [Fin[oms](../api/user-findrooms.md)は、テナント内の最初の100ルームに戻る |
|テナント内の[個別の会議室または会議室一覧の取得](../api/place-get.md)をサポートしています。 | テナント内の個別の会議室または会議室一覧の取得はサポートされていません
|表示名と SMTP アドレスに加えて、豊富なプロパティセットを指定する[room](room.md)および[roomList](roomlist.md)の特定のエンティティを定義します。 | 各会議室および会議室一覧には、表示名と SMTP アドレスのみを指定する、軽量化された[emailAddress](emailaddress.md)の種類があります。|
|委任 (職場または学校のアカウント) またはアプリケーションのアクセス許可を持つ、組織のシナリオのみをサポートします。 | 委任されたアクセス許可またはアプリケーションのアクセス許可を持つ組織のシナリオに対して同様のサポート|

## <a name="methods"></a>メソッド

| メソッド                              | 戻り値の型                  | 説明 |
|:------------------------------------|:-----------------------------|:--------|
| [プレースを一覧表示する](../api/place-list.md) | 要求された派生型のコレクション。 [](place.md) | テナントで定義されている、指定された種類の**プレース**オブジェクトのコレクションを取得します。 |
| [場所を取得する](../api/place-get.md)    | 要求された派生型[](place.md)            | 指定した**place**オブジェクトのプロパティとリレーションシップを取得します。 |

## <a name="properties"></a>プロパティ

| プロパティ       | 型                                              | 説明 |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | 場所の住所。 |
| displayName    | String                                            | 場所に関連付けられている名前。 |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 緯度、経度、および (オプションで) 高度座標での場所を指定します。 |
| id             | 文字列                                            | 場所の一意識別子。 読み取り専用です。 |
| phone          | String                                            | 場所の電話番号。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "id": "String (identifier)",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "phone": "String"
}
```

## <a name="see-also"></a>関連項目
- 管理者が会議室一覧を作成するには、Exchange PowerShell コマンドレットの[新しいグループ](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps)を使用します。
- 管理者が会議室一覧に会議室を追加するには、Exchange Powershell コマンドレット[get-distributiongroupmember](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps)を使用します。

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
