---
title: governanceResource リソースの種類
description: 特権を持つユーザー情報管理 (PIM) で管理できるリソースを表します。 Azure のリソースでは、サブスクリプション、リソース グループ、およびなど、仮想マシン、SQL データベースなどのリソースとなります。
localization_priority: Normal
ms.openlocfilehash: 263996049753256fd39906dba61138c3ab0f0248
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869392"
---
# <a name="governanceresource-resource-type"></a>governanceResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特権を持つユーザー情報管理 (PIM) で管理できるリソースを表します。 Azure のリソースでは、サブスクリプション、リソース グループ、およびなど、仮想マシン、SQL データベースなどのリソースとなります。


## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [governanceResource](../resources/governanceresource.md)コレクション|リクエスターへのアクセス権を持つリソースの一覧を表示します。|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Id で指定されたリソースのエンティティのプロパティと関係を参照してください。|
|[登録](../api/governanceresource-register.md) | |アンマネージ Azure サブスクリプションまたは管理グループに PIM サービスを登録します。 |

No `POST`、 `PUT`、 `PATCH`、`DELETE`でサポートされている`roleDefinitions`ここではエンティティのセットです。

## <a name="properties"></a>プロパティ
| プロパティ          |種類         |説明|
|:------------------|:----------|:----------|
|ID                 |String     |リソースの id です。 GUID 形式であります。|
|externalId           |String   |外部システムで、元の id を表すリソースの外部の id です。 たとえば、サブスクリプション リソースの外部 id には、「サブスクリプション/c14ae696-5e0c-4e5d-88cc-bef6637737ac」ができます。 |
|type               |String     |必須。 リソースの種類。 たとえば、Azure のリソースの種類可能性があります「サブスクリプション」、「リソース グループ」、"Microsoft.Sql/server"など。|
|displayName        |String     |リソースの表示名。|
|status             |String     |特定のリソースの状態です。 たとえば、リソースをロックするかどうかを表すことが、(値: `Active` / `Locked`)。 メモ: このプロパティ拡張することが、将来的に複数のシナリオをサポートします。|
|registeredDateTime|DateTimeOffset      |PIM にリソースを登録するときの日時を表します。|
|registeredRoot|String      |PIM に登録されているリソースのルート スコープの externalId です。 ルート スコープには、親、親の親、または先祖の高いリソースができます。|
|roleAssignmentCount|Int32      |省略可能。 特定のリソースに対するロールの割り当ての数です。 プロパティを取得するには、明示的に使用をしてください。`$select=roleAssignmentCount`クエリにします。|
|roleDefinitionCount|Int32      |省略可能。 指定されたリソースの役割の定義の数です。 プロパティを取得するには、明示的に使用をしてください。`$select=roleDefinitionCount`クエリにします。|
|permissions|[governancePermission](../resources/governancepermission.md)      |省略可能。 リソースへのアクセスの要求元の状態を表します。プロパティを取得するには、明示的に使用をしてください。`$select=permissions`クエリにします。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ   | 型                                         |説明|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション|リソースに対するロールの割り当てのコレクションです。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md)コレクション|リソースのロール定義のコレクションです。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション|リソースの役割の割り当て要求のコレクションです。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md)コレクション|リソースのロールの設定のコレクションです。|
|親          |[governanceResource](../resources/governanceresource.md)           |読み取り専用です。 親リソースです。 `pimforazurerbac`シナリオでは、サブスクリプションに属しているリソースを表すことができます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
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
  "registeredRoot": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
