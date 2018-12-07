---
title: governanceRoleAssignmentRequest リソースの種類
description: Privilegd Id 管理の役割の割り当て操作の要求を表します。
ms.openlocfilehash: b3f3c7b3ec324b9b3df24cc0c53eaa6d1cda7a4c
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191124"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>governanceRoleAssignmentRequest リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Privilegd Id 管理の役割の割り当て操作の要求を表します。

`governanceRoleAssignmentRequest`チケット モデルのエンティティはロールの割り当てのライフ サイクルを管理するために使用されます。 ・繰り返し schduling、承認のゲートを直接公開するのと比較した場合のように実装を有効にする柔軟性も提供してユーザーや管理者などの意図と意思決定を表す`POST`、 `PUT`、および`DELETE`の操作`governanceRoleAssignment`。

## <a name="methods"></a>Methods

| メソッド          |戻り値の型  |説明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|ID で指定されたロールの割り当て要求を取得します。  
|[List](../api/governanceroleassignmentrequest-list.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション|リソースの役割の割り当て要求を取得します。|
|[作成](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|既存または新しい役割の割り当てのライフ サイクルを管理するために要求を作成します。|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |保留中の役割の割り当て要求をキャンセルします。|
|[Update](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|管理者は、要求の状態の場合に要求の決定を更新`PendingAdminDecision`。|

## <a name="properties"></a>プロパティ
| プロパティ                  | 種類          |説明|
|:--------------------------|:--------------|:----------|
|id                         |String         |役割の割り当て要求の id。|
|resourceId                 |String         |必須。 役割の割り当て要求に関連付けられているリソースの id です。|
|roleDefinitionId           |String         |必須。 役割の割り当て要求に関連付けられている役割の定義の id です。|
|subjectId                  |String         |必須。 役割の割り当て要求に関連付けられているサブジェクトの id です。|
|type                       |String         |必須。 表す、ロールの割り当ての操作の種類です。 値は、します。 <ul><li>`AdminAdd`: 管理者の役割にユーザーまたはグループを割り当てる</li><li>`UserAdd`: ユーザーが対象の割り当てを有効化します。</li><li> `AdminUpdate`: 管理者は、既存のロールの割り当てを変更します。</li><li>`AdminRemove`: 管理者の役割からユーザーまたはグループを削除します。<li>`UserRemove`: ユーザーは、作業中の割り当てを非アクティブ化します。<li>`UserExtend`: ユーザーが、有効期限切れの割り当てを拡張する要求します。</li><li>`AdminExtend`: 管理者は、期限切れの割り当てを拡張します。</li><li>`UserRenew`: ユーザーの要求が期限切れの割り当てを更新するには</li><li>`AdminRenew`: 管理者は、期限切れの割り当てを拡張します。</li></ul>|
|assignmentState|String  |必須。 割り当ての状態です。 値は、します。 <ul><li> `Eligible`対象となる割り当ての</li><li> `Active`-直接割り当てられている場合`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</li></ul>|
|requestedDateTime          |DateTimeOffset |取得のみ可能な値です。 要求は、時間を作成します。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|スケジュール                   |[governanceSchedule](governanceschedule.md)|役割の割り当て要求のスケジュール オブジェクトです。|
|理由                     |String         |ユーザーおよび管理者によって提供されるメッセージが必要な理由についての要求を作成するとします。|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |役割の割り当て要求のステータス。|
|linkedEligibleRoleAssignmentId|String        |Id を表すロールのアクティブ化の要求の場合は、`eligible assignment`で参照されます。値は、それ以外の場合、 `null`。 |



## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型                                |説明|
|:-------------|:----------------------------------|:----------|
|リソース      |[governanceResource](../resources/governanceresource.md)            |取得のみ可能な値です。 要求することを目的とするリソースです。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|取得のみ可能な値です。 役割の定義を要求することを目的とします。 |
|subject       |[governanceSubject](../resources/governancesubject.md)|取得のみ可能な値です。 ユーザ/グループのプリンシパルです。|

### <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "type": "String",
  "assignmentState": "String",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
