---
title: administrativeUnit リソースの種類
description: 管理単位は、ユーザーおよびグループのディレクトリオブジェクトの概念コンテナーを提供します。 管理単位を使用することで、会社の管理者は、管理単位に含まれるユーザーやグループを管理するための管理責任を、地域または部門の管理者に委任できるようになりました。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 507b74a32a175bfc37405bd66ddef6f5bfa49c9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013466"
---
# <a name="administrativeunit-resource-type"></a>administrativeUnit リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

管理単位は、ユーザーおよびグループのディレクトリオブジェクトの概念コンテナーを提供します。 管理単位を使用することで、会社の管理者は、管理単位に含まれるユーザーやグループを管理するための管理責任を、地域または部門の管理者に委任できるようになりました。

1 つの例を見てみましょう。 Contoso Corp が2つの部署で構成されていると仮定します。たとえば、West 海岸部と東海岸部があります。 Contoso 社のディレクトリの役割は、テナント全体に適用されます。 Contoso 社の管理者である Lee は、管理責任を委任しようとしていますが、西海岸部または東海岸部に適用されます。  Lee は、*西海岸 admistrative ユニット*を作成し、すべての west 沿岸ユーザーをこの管理単位に配置できます。  同様に、Lee では、*東海岸管理ユニット*を作成できます。  Lee では、管理者の責任を他のユーザーに委任することはできますが、作成した新しい管理単位に**スコープ**を設定することができます。 Lee は、*ヘルプデスク管理者*の**** 役割を持つ Jennifer を*West Coast 管理単位*に配置します。  これにより、Jennifer はユーザーのパスワードをリセットすることができますが、それらのユーザーが*West Coast 管理単位*にいる場合に限られます。  同様に、Lee は、*東海岸管理単位*を対象**範囲**とする*ユーザーアカウント管理者*の役割で Dave を設定します。  これにより、Dave はユーザーの更新、ライセンスの割り当て、ユーザーのパスワードのリセットを行うことができます。ただし、ユーザーが*東海岸の管理単位*にいる場合に限ります。 ビデオの概要については、「 [Azure Active Directory の管理単位の概要」を](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)参照してください。

このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。

このトピックでは、administrativeUnit エンティティによって公開される宣言されたプロパティとナビゲーションプロパティについて説明するほかに、Group や directoryrole リソースで呼び出すことができる操作と関数についても説明します。


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[AdministrativeUnit を作成する](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | 新しい管理単位を作成します。|
|[リスト Group や directoryrole](../api/administrativeunit-list.md) | [administrativeUnit](administrativeunit.md)コレクション |すべての Group や directoryrole のプロパティを一覧表示します。|
|[AdministrativeUnit を取得する](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |特定の administrativeUnit オブジェクトのプロパティとリレーションシップを読み取ります。|
|[AdminstrativeUnit の更新](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)  |AdministrativeUnit オブジェクトを更新します。 |
|[AdminstrativeUnit の削除](../api/administrativeunit-delete.md) | None |AdministrativeUnit オブジェクトを削除します。 |
|[Add a member](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| メンバー (ユーザーまたはグループ) を追加します。|
|[メンバーを一覧表示する](../api/administrativeunit-list-members.md) |[directoryObject](directoryobject.md) コレクション| (ユーザーおよびグループ) メンバーの一覧を取得します。|
|[メンバーを取得する](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| 特定のメンバーを取得します。|
|[メンバーを削除する](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| メンバーを削除します。|
|[スコープロールのメンバーを追加する](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| スコープ付きの役割メンバーを追加します。|
|[スコープが指定された役割のメンバーを一覧表示する](../api/administrativeunit-list-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md) コレクション| スコープの役割を持つ管理者の一覧を取得します。|
|[スコープロールのメンバーを取得する](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 特定の範囲の役割メンバーを取得します。|
|[スコープ指定された役割メンバーを削除する](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| スコープ指定された役割メンバーを削除します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|description|string|管理単位の説明 (オプション)。|
|displayName|string|管理単位の表示名。|
|id|文字列|管理単位の一意の識別子。 読み取り専用です。|
|visibility|string|管理単位とそのメンバーを非表示にするか、または公開するかを制御します。 HiddenMembership または Public に設定できます。 設定されていない場合、既定の動作はパブリックになります。 HiddenMembership に設定されている場合、管理単位のメンバーのみが、管理単位の他のメンバーを一覧表示できます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|extensions|[extension](extension.md) コレクション|この管理単位に対して定義されているオープン拡張機能のコレクション。 Null 許容型。|
|members|[directoryObject](directoryobject.md) コレクション|この Adminsitrative Unit のメンバーであるユーザーとグループ。 HTTP メソッド: GET (メンバーの一覧)、POST (メンバーの追加)、削除 (メンバーの削除)。|
|scopedRoleMembers|[scopedRoleMembership](scopedrolemembership.md) コレクション| スコープ-この管理単位の役割メンバー。  HTTP メソッド: GET (list scopedRoleMemberships)、POST (add scopedRoleMembership)、DELETE (remove scopedRoleMembership)。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
