---
title: privilegedRoleAssignmentRequest リソースの種類
description: Privilegd Identity Management での役割の割り当て操作の要求を表します。
localization_priority: Normal
ms.openlocfilehash: 240c84ecb0bf4f8d0e171f647f21eb6730c28d44
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621215"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>privilegedRoleAssignmentRequest リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Privilegd Identity Management での役割の割り当て操作の要求を表します。

`privilegedRoleAssignmentRequest`は、役割の割り当てのライフサイクルを管理するために使用される、チケットモデル化されたエンティティです。 これは、ユーザーと管理者の意図または決定を表し、さらに、定期的な schduling の実装、承認ゲートの実装を可能にする柔軟性を備えて`POST`い`LIST`ます。また、直接の公開と操作に加えて、`MY`と`Cancel`の機能`governanceRoleAssignment`をオンにします。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)コレクション|役割の割り当て要求を一覧表示します。|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|既存または新しい役割の割り当てのライフサイクルを管理するための要求を作成します。|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |保留中の役割の割り当て要求を取り消します。|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |現在の requstor に対する役割の割り当て要求を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|id|String| 読み取り専用です。 役割の割り当て要求の id。|
|割り当ての状態|String| 割り当ての状態を指定します。 この値は、 `Eligible`管理者に`Active`よって直接割り当てら`Active`れている場合、またはユーザーによる資格のある割り当てに対してアクティブ化されている場合に、対象となる割り当てに使用できます。|
|duration|String| 役割の割り当ての期間。|
|したがっ|String| 役割の割り当ての理由。|
|requestedDateTime|DateTimeOffset| 読み取り専用。 要求の作成時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|roleId|String| ロールの id。|
|schedule|[governanceSchedule](governanceschedule.md)| 役割の割り当て要求の schedule オブジェクト。|
|status|文字列型 (String)| 読み取り専用。役割の割り当て要求の状態。 値`NotStarted``Completed``Revoked``RequestExpired`は、、、、、、、、、、、のようになります。`RequestedApproval``Scheduled``Approved``ApprovalDenied``ApprovalAborted``Cancelling``Cancelled`|
|ticketNumber|String| 役割の割り当ての ticketNumber。 |
|ticketSystem|String| 役割の割り当ての ticketSystem。|
|type|String| 役割の割り当てに対する操作の種類を表します。 値は次の`AdminAdd`ようになります。「ユーザーを役割に追加する」。`UserAdd`: ユーザーが役割の割り当てを追加します。|
|userId|String| ユーザーの id。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| 役割の割り当て要求の roleInfo オブジェクト。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
