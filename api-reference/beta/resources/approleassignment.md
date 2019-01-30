---
title: appRoleAssignment リソースの種類
description: ユーザーまたはグループがアプリケーションに割り当てられるときの記録に使用します。 この例では、ロールの割り当てにより、アプリケーション タイルが、ユーザー アプリケーションのアクセス パネル上に表示されます。 特定のロールで、リソース アプリケーションに別の (サービス プリンシパルとしてモデル化された) アプリケーションのアクセス権を付与する場合にも、このエンティティを使用できます。 ロールの割り当ての作成、読み取り、更新、削除ができます。
localization_priority: Priority
ms.openlocfilehash: 4e4bb6e2c9f94780dba642167ecdb9200849038f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576620"
---
# <a name="approleassignment-resource-type"></a>appRoleAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーまたはグループがアプリケーションに割り当てられるときの記録に使用します。 この例では、ロールの割り当てにより、アプリケーション タイルが、ユーザー アプリケーションのアクセス パネル上に表示されます。 特定のロールで、リソース アプリケーションに別の (サービス プリンシパルとしてモデル化された) アプリケーションのアクセス権を付与する場合にも、このエンティティを使用できます。 ロールの割り当ての作成、読み取り、更新、削除ができます。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|creationTimestamp|DateTimeOffset|許可が出された時間です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|Guid|プリンシパルに割り当てられたロール ID です。  このロールは、**appRoles** プロパティのターゲット リソース アプリケーション **resourceId** によって宣言される必要があります。 リソースがアクセス許可を宣言していない場合は、既存の ID (ゼロ GUID) を指定する必要があります。 キー。 null 許容型ではありません。 |
|principalDisplayName|String|アクセス権が付与されているプリンシパルの表示名。|
|principalId|Guid|アクセス権が付与されているプリンシパルの一意の識別子 (**id**) です。 作成時に必要です。            |
|principalType|String|プリンシパルの種類。  "User"、"Group"、"ServicePrincipal" のいずれかを指定できます。|
|resourceDisplayName|String|割り当てが作成されたリソースの表示名。|
|resourceId|Guid|割り当てが作成されたターゲット リソース (サービス プリンシパル) の一意の識別子 (**id**) です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[appRoleAssignment を取得する](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |appRoleAssignment オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/approleassignment-update.md) | [appRoleAssignment](approleassignment.md)   |appRoleAssignment オブジェクトを更新します。 |
|[削除する](../api/approleassignment-delete.md) | なし |appRoleAssignment オブジェクトを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
