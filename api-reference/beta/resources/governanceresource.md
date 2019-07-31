---
title: governanceResource リソースの種類
description: 特権 Id 管理 (PIM) によって管理される可能性があるリソースを表します。 Azure リソースの場合は、サブスクリプション、リソースグループ、仮想マシン、SQL データベースなどのリソースを使用できます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a0429de2cacc816eaf1a603a29a08897650da6e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971922"
---
# <a name="governanceresource-resource-type"></a>governanceResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権 Id 管理 (PIM) によって管理される可能性があるリソースを表します。 Azure リソースの場合は、サブスクリプション、リソースグループ、仮想マシン、SQL データベースなどのリソースを使用できます。


## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [governanceResource](../resources/governanceresource.md)コレクション|要求者がアクセスできるリソースのコレクションを一覧表示します。|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Id で指定されたリソースエンティティのプロパティとリレーションシップを読み取ります。|
|[登録](../api/governanceresource-register.md) | |管理されていない Azure サブスクリプションまたは管理グループを PIM サービスに登録します。 |

`PATCH` `roleDefinitions`現時点では、entity set ではサポートされていません`POST` `PUT` `DELETE`

## <a name="properties"></a>プロパティ
| プロパティ          |型         |説明|
|:------------------|:----------|:----------|
|id                 |文字列     |リソースの id。 GUID 形式です。|
|externalId           |String   |外部システムの元の id を表す、リソースの外部 id。 たとえば、サブスクリプションリソースの外部 id は "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac" にすることができます。 |
|type               |String     |必須。 リソースの種類。 たとえば、Azure リソースの場合、この型は "Subscription"、"ResourceGroup"、"Microsoft .Sql/server" などになります。|
|displayName        |String     |リソースの表示名。|
|status             |String     |指定されたリソースの状態。 たとえば、リソースがロックされているかどうかを表すことが`Active` / `Locked`できます (値:)。 注: 今後、このプロパティを拡張して、より多くのシナリオをサポートすることができます。|
|registeredDateTime|DateTimeOffset      |リソースが PIM に登録されている日時を表します。|
|registeredRoot|String      |PIM に登録されているリソースのルートスコープの externalId。 ルートスコープには、親、親、または上位の先祖リソースを指定できます。|
|Role割り当て数|Int32      |省略可能。 指定したリソースのロール割り当ての数。 プロパティを取得するには、クエリ`$select=roleAssignmentCount`で明示的にを使用してください。|
|roleDefinitionCount|Int32      |省略可能。 指定したリソースのロール定義の数。 プロパティを取得するには、クエリ`$select=roleDefinitionCount`で明示的にを使用してください。|
|アクセス許可|[governancePermission](../resources/governancepermission.md)      |省略可能。 これは、リソースへの要求者のアクセスの状態を表します。プロパティを取得するには、クエリ`$select=permissions`で明示的にを使用してください。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ   | 型                                         |説明|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション|リソースのロール割り当てのコレクション。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション|リソースのロール日のコレクション。|
|Rolerequests 要求 |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション|リソースに対する役割の割り当て要求のコレクション。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md)コレクション|リソースのロール設定のコレクション。|
|親行          |[governanceResource](../resources/governanceresource.md)           |読み取り専用です。 親リソース。 シナリオ`pimforazurerbac`の場合は、リソースが属するサブスクリプションを表すことができます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String",
  "roleAssignmentCount": 12356,
  "roleDefinitionCount": 12356,
  "permissions": {
    "@odata.type": "microsoft.graph.governancePermission"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
