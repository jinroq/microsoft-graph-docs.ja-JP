---
title: governanceRoleSetting リソースの種類
description: " ルールというように。"
ms.openlocfilehash: 64245b2d6f0aa9e0ea3ffda4a5eaebfb9fd205df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070765"
---
# <a name="governancerolesetting-resource-type"></a>governanceRoleSetting リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

各役割の割り当ての作成または変更されたときに、に対して評価する必要がある役割の定義の構成のセットを表します。 たとえば、ロールの設定は、[最大割り当て期間] のルール、ルールの「ライセンス認証に必要な MFA」などがあります。

## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | [governanceRoleSetting](../resources/governancerolesetting.md)コレクション|リソースのロールの設定の一覧を表示します。|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |ロール設定のプロパティと関係を参照してください。|
|[Update](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |ロールの設定オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
|プロパティ               |型                                      |説明|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |RoleSetting の id です。|
|resourceId           |String                                  |必須。 役割の設定が関連付けられているリソースの id です。|
|roleDefinitionId     |String                                  |必須。 役割の設定が関連付けられている役割の定義の id です。|
|isDefault            |ブール値                                 |読み取り専用。 RoleSetting がデフォルトの roleSetting であることを示す|
|lastUpdatedDateTime  |DateTimeOffset                          |読み取り専用。 役割の設定が最後に更新された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|lastUpdatedBy        |String                                  |読み取り専用。 RoleSetting を最後に更新した管理者の表示名。|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|管理者対象のロール割り当てを追加しようとするときに評価されるルールの設定。|
|adminMemberSettings  |[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|直接的なメンバーの役割の割り当てを追加する際に管理者に評価されるルールの設定。|
|userEligibleSettings |[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|ユーザーが対象のロール割り当てを追加するときに評価されるルールの設定。 設定は、ここではサポートされていません。|
|userMemberSettings   |[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|ユーザーが彼の役割の割り当てを有効にしようとした場合に評価されるルールの設定。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用。 このロールの設定に関連付けられているリソースです。|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|読み取り専用。 役割の定義を適用するこのロールの設定をします。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
