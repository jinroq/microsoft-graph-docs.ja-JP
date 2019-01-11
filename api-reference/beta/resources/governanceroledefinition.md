---
title: governanceRoleDefinition リソースの種類
description: 役割の定義を表します。 Azure のリソースの所有者、閲覧者、投稿者など、Azure の RBAC の役割を表すことができます。
localization_priority: Normal
ms.openlocfilehash: 3f94dd1a741545760951875fbc064307823a65dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842451"
---
# <a name="governanceroledefinition-resource-type"></a>governanceRoleDefinition リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。 


役割の定義を表します。 Azure のリソースの所有者、閲覧者、投稿者など、Azure の RBAC の役割を表すことができます。


## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション |リソースの役割の定義の一覧を表示します。|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Id で指定されたロールの定義のエンティティのプロパティと関係を参照してください。|
No `POST`、 `PUT`、 `PATCH`、`DELETE`でサポートされています`roleDefinitions`ここではエンティティのセットです。
## <a name="properties"></a>プロパティ
| プロパティ  | 種類      |説明|
|:----|:----------|:----------|:----------|
|ID         |String     |役割の定義の id です。 |
|resourceId |String     |必須。 役割の定義に関連付けられているリソースの id です。 |
|externalId   |String     |役割の定義の外部の id です。|
|displayName|String     |役割の定義の表示名。|
|subjectCount|Int32     |省略可能。 ロールに割り当てられている被験者の数です。 リソースへのアクセスの要求元の状態を表します。 プロパティを取得するには、明示的に使用をしてください。`$select=subjectCount`クエリにします。|
|eligibleAssignmentCount|Int32|省略可能。 役割の定義に関連付けられている対象のロールの割り当ての数です。 プロパティを取得するには、明示的に使用をしてください。`$select=eligibleAssignmentCount`クエリにします。|
|activeAssignmentCount|Int32    |省略可能。 役割の定義に関連付けられているアクティブなロールの割り当ての数です。  プロパティを取得するには、明示的に使用をしてください。`$select=activeAssignmentCount`クエリにします。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用です。 役割の定義に関連付けられているリソースです。|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|役割の定義に関連付けられている役割の設定をします。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
