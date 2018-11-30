---
title: privilegedRoleAssignmentRequest リソースの種類
description: Privilegd Id 管理の役割の割り当て操作の要求を表します。
ms.openlocfilehash: b715c88157a7df52dabcb4c746dfe70bc2523d18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072922"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>privilegedRoleAssignmentRequest リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Privilegd Id 管理の役割の割り当て操作の要求を表します。

`privilegedRoleAssignmentRequest`チケット モデルのエンティティはロールの割り当てのライフ サイクルを管理するために使用されます。 ・繰り返し schduling、承認のゲートを直接公開するのと比較した場合のように実装を有効にする柔軟性も提供してユーザーや管理者などの意図と意思決定を表す`POST`と`LIST`の操作だけでなく`MY`と`Cancel`の機能`governanceRoleAssignment`。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)コレクション|役割の割り当て要求を一覧表示します。|
|[作成](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|既存または新しい役割の割り当てのライフ サイクルを管理するために要求を作成します。|
|[キャンセル](../api/privilegedroleassignmentrequest-cancel.md)|  |保留中の役割の割り当て要求をキャンセルします。|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |現在の requstor の役割の割り当て要求を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|id|String| 読み取り専用。 役割の割り当て要求の id。|
|assignmentState|String| 割り当ての状態です。 値は、`Eligible`対象となる割り当ての`Active`が直接割り当てられている場合 -`Active`管理者、またはユーザーが対象となる割り当ての有効化します。|
|duration|String| 役割の割り当ての期間です。|
|理由|String| ロールの割り当ての理由です。|
|requestedDateTime|DateTimeOffset| 読み取り専用。 要求は、時間を作成します。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|roleId|String| ロールの id です。|
|スケジュール|[governanceSchedule](governanceschedule.md)| 役割の割り当て要求のスケジュール オブジェクトです。|
|status|String| 役割の割り当て要求の読み取り only.The 状態です。 値は、 `NotStarted`、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。|
|ticketNumber|String| ロールの割り当てを ticketNumber。 |
|ticketSystem|String| ロールの割り当てを ticketSystem。|
|type|String| 表す、ロールの割り当ての操作の種類です。 値は、 `AdminAdd`: 管理者のユーザー ロールを追加します。`UserAdd`: ユーザーは、役割の割り当てを追加します。|
|userId|String| ユーザーの id です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| 役割の割り当て要求の roleInfo オブジェクトです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->