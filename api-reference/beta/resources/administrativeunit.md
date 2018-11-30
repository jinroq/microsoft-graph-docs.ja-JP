---
title: administrativeUnit リソースの種類
description: 管理単位は、ユーザーとグループのディレクトリ オブジェクトの概念的なコンテナーを提供します。 管理単位を使用すると、企業の管理者はユーザーを管理する管理責任を委任できるようになりましたと、グループ内に含まれている、地域や部門の管理者に管理単位にスコープを設定しました。
ms.openlocfilehash: 8c0acd25c231707d2a7188ab2e1c2b0d2035816f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066518"
---
# <a name="administrativeunit-resource-type"></a>administrativeUnit リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

管理単位は、ユーザーとグループのディレクトリ オブジェクトの概念的なコンテナーを提供します。 管理単位を使用すると、企業の管理者はユーザーを管理する管理責任を委任できるようになりましたと、グループ内に含まれている、地域や部門の管理者に管理単位にスコープを設定しました。

例を見てみましょう。 -西海岸の部門および東海岸の事業部の 2 つの部門の構成が contoso 社の会社を想像してください。 ディレクトリの役割を contoso 社では、全体のテナントに適用されます。 Lee、contoso 社の企業の管理者は、管理責任を委任するスコープを設定して、西海岸事業部や東海岸の部門を希望しています。  Lee では、*西海岸の admistrative ユニット*を作成でき、西海岸のすべてのユーザーをこの管理単位に配置することができます。  同様に、Lee は、*東海岸の管理単位*を作成できます。  Lee は、他のユーザーに管理責任を委任することを開始できるようになりましたが、**スコープ**の新規の管理単位に彼が作成されます。 Lee は、*ヘルプデスク管理者*ロールの**スコープ**に*西海岸の管理単位*で Jennifer を配置します。  これにより、*西海岸の管理単位*でそれらのユーザーがいる場合にのみ、すべてのユーザーのパスワードをリセットするのには Jennifer。  同様に、Lee は、*ユーザー アカウントの管理者*ロールの**スコープ**に*東海岸の管理単位*でのデイブを配置します。  これにより、ユーザーの更新、ライセンスを割り当てるし、のみ場合は、*東海岸の管理単位*では、すべてのユーザーのパスワードをリセットする Dave。 ビデオについては、 [Azure Active Directory の管理単位の概要](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)を参照してください。

このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。

このトピックでは、宣言されたプロパティと、administrativeUnit のエンティティと同様に操作と administrativeUnits リソースを呼び出すことができる関数によって公開されているナビゲーション プロパティの説明を示します。


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[AdministrativeUnit を作成します。](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | 新規の管理単位を作成します。|
|[リスト administrativeUnits](../api/administrativeunit-list.md) | [administrativeUnit](administrativeunit.md)コレクション |AdministrativeUnits のすべてのプロパティを一覧表示します。|
|[Get administrativeUnit](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |特定の administrativeUnit オブジェクトのプロパティと関係を参照してください。|
|[AdminstrativeUnit を更新します。](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)  |AdministrativeUnit オブジェクトを更新します。 |
|[AdminstrativeUnit を削除します。](../api/administrativeunit-delete.md) | なし |AdministrativeUnit オブジェクトを削除します。 |
|[メンバーを追加する](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| (ユーザーまたはグループ) のメンバーを追加します。|
|[メンバーを一覧表示する](../api/administrativeunit-list-members.md) |[directoryObject](directoryobject.md) コレクション| (ユーザーおよびグループ) のメンバーの一覧を取得します。|
|[メンバーを取得します。](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| 特定のメンバーを取得します。|
|[メンバーを削除する](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| メンバーを削除します。|
|[スコープ ロール メンバーを追加します。](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| スコープ ロールのメンバーを追加します。|
|[スコープ ロールのメンバーの一覧](../api/administrativeunit-list-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md) コレクション| スコープ ロールの管理者の一覧を取得します。|
|[スコープ ロールのメンバーを取得します。](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 特定のスコープにロールのメンバーを取得します。|
|[スコープ ロール メンバーを削除します。](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| スコープ ロールのメンバーを削除します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|文字列|管理単位のオプションの説明です。|
|displayName|string|管理単位の名前を表示します。|
|ID|文字列|管理単位の一意の識別子です。 読み取り専用。|
|visibility|文字列|またはパブリック フォルダー管理の単位とそのメンバーが非表示かどうかを制御します。 HiddenMembership またはパブリックに設定できます。 ない場合、既定の動作のセット公開。 管理の単位のメンバーだけの HiddenMembership に設定すると、管理単位の他のメンバーが一覧表示できます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|extensions|[extension](extension.md) コレクション|この管理単位に定義されている、開いている拡張機能のコレクションです。 Null 許容型。|
|members|[directoryObject](directoryobject.md) コレクション|ユーザーとグループがこの Adminsitrative ユニットのメンバーであります。 HTTP メソッド: 投稿 (メンバーの一覧) を取得 (メンバー) を追加 (メンバーの削除) を削除します。|
|scopedRoleMembers|[scopedRoleMembership](scopedrolemembership.md) コレクション| この管理単位のスコープにロールのメンバーです。  HTTP メソッド: 投稿 (リスト scopedRoleMemberships) を取得 (scopedRoleMembership)、追加 (削除 scopedRoleMembership) を削除します。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.administrativeUnit"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "visibility": "string"
}

```


## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->