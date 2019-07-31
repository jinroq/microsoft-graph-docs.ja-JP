---
title: governanceRoleAssignment リソースの種類
description: ユーザーまたはグループの役割への割り当てを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 518fbe18fcd09b1b4cc9730c6b7f0112adabfeae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971894"
---
# <a name="governanceroleassignment-resource-type"></a>governanceRoleAssignment リソースの種類
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーまたはグループの役割への割り当てを表します。

Privileged Identity Management (PIM) は、次の2種類の割り当てをサポートしています。

1. アクティブな割り当て-リソースへの直接/アクティブ化されたアクセスを表します。
2. 対象となる割り当て-リソースへの特権アクセスの中間段階であり、アクセスなしと直接アクセスの間の関係を表します。 管理者は、ユーザーまたは`eligible assignment`グループを事前に割り当てることができます。 `activation`また、 `eligible assignment`アクセスが必要になったときに、に対して、で数時間にリソースへの即時アクセスを取得する必要があります。 アクティブ化した`active assignment`後、ユーザー/グループメンバーに対してが作成され、アクティブ化された状態を示します。

## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |役割割り当てエンティティのプロパティと関係を読み取ります。|
|[List](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション|リソースに対する役割の割り当てのコレクションを一覧表示します。 |
|[Export](../api/governanceroleassignment-export.md) | オクテットストリーム |リソースに対する役割の割り当てのコレクションをダウンロードし、 `.csv`ファイルとして保存します。|

`PATCH` `DELETE` `POST` `PUT`エンティティセットでは、、、、または操作はサポートされていません。 `roleAssignments` の`governanceRoleAssignment`作成、更新、および削除操作は、によっ`governanceRoleAssignmentRequest`て実行されます。

## <a name="properties"></a>プロパティ
| プロパティ  | 型      |説明|
|:----------|:----------|:----------|
|id         |文字列     |役割の割り当ての ID。 GUID 形式です。|
|resourceId |String     |必須。 役割の割り当てが関連付けられているリソースの ID。 |
|roleDefinitionId|String|必須。 役割の割り当てが関連付けられているロール定義の ID。 |
|subjectId|String       |必須。 役割の割り当てが関連付けられているサブジェクトの ID。 |
|linkedEligibleRoleAssignmentId|String|が`active assignment`で、アクティブ化によって作成され`eligible assignment`たものである場合は、 `eligible assignment`その ID を表します。それ以外の場合、 `null`値はです。 |
|externalId   |String     |プロバイダーでの役割の割り当てを識別するために使用されるリソースの、外部 ID。|
|startDateTime|DateTimeOffset|役割の割り当ての開始時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|非永続的な役割の割り当ての場合、これは、役割の割り当てが期限切れになる時刻です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|割り当ての状態|String  |割り当ての状態を指定します。 値には、 <ul><li> `Eligible`適格な割り当ての場合</li><li> `Active`-管理者によって`Active`直接割り当てられている場合、またはユーザーによる資格のある割り当てでアクティブ化されている場合。</li></ul>|
|memberType|String      |メンバーの種類を示します。 値は次のようになります。 <ul><li>`Inherited`-役割の割り当ては、親のリソーススコープから継承されます。</li><li>`Group`-役割の割り当ては継承されませんが、グループの割り当てのメンバーシップから取得されます。</li><li>`User`-役割の割り当ては、継承されたものでも、グループの割り当てにもありません。</li></ul>|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用です。 役割の割り当てに関連付けられているリソース。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|読み取り専用です。 役割の割り当てに関連付けられている役割の定義。 |
|subject|[governanceSubject](../resources/governancesubject.md)|読み取り専用です。 役割の割り当てに関連付けられている件名。 |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|読み取り専用です。 が`active assignment`で、アクティブ化のために作成され`eligible assignment`ている場合は、そのオブジェクト`eligible assignment`を表します。それ以外の場合、 `null`値はです。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
