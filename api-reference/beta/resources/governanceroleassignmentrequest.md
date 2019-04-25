---
title: governanceRoleAssignmentRequest リソースの種類
description: Privilegd Identity Management での役割の割り当て操作の要求を表します。
localization_priority: Normal
ms.openlocfilehash: 242f1d311a2d304d0d8dab0a4e24f9294722ab6e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547455"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>governanceRoleAssignmentRequest リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Privilegd Identity Management での役割の割り当て操作の要求を表します。

`governanceRoleAssignmentRequest`は、役割の割り当てのライフサイクルを管理するために使用される、チケットモデル化されたエンティティです。 ユーザーと管理者の意図または決定を表しており、直接公開`POST`、 `PUT`および`DELETE`操作と比較して、定期的な schduling、承認ゲートなどの実装を可能にする柔軟性も提供します。オン`governanceRoleAssignment`にします。

## <a name="methods"></a>メソッド

| メソッド          |戻り値の型  |説明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|ID で指定された役割の割り当て要求を取得します。  
|[List](../api/governanceroleassignmentrequest-list.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)コレクション|リソースに対して役割の割り当て要求を取得します。|
|[作成](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|既存または新しい役割の割り当てのライフサイクルを管理するための要求を作成します。|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |保留中の役割の割り当て要求を取り消します。|
|[更新](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|要求がの`PendingAdminDecision`状態にある場合、管理者は要求に関する決定を更新します。|

## <a name="properties"></a>プロパティ
| プロパティ                  | 型          |説明|
|:--------------------------|:--------------|:----------|
|id                         |String         |役割の割り当て要求の id。|
|resourceId                 |String         |必須。 役割の割り当て要求が関連付けられているリソースの id。|
|roleDefinitionId           |String         |必須。 役割の割り当て要求が関連付けられているロール定義の id。|
|subjectId                  |String         |必須。 役割の割り当て要求が関連付けられているサブジェクトの id。|
|type                       |String         |必須。 役割の割り当てに対する操作の種類を表します。 値には、 <ul><li>`AdminAdd`: ユーザー/グループを役割に割り当てる。</li><li>`UserAdd`: ユーザーが適格な割り当てをアクティブにします。</li><li> `AdminUpdate`: 既存の役割の割り当ての変更を行う</li><li>`AdminRemove`: [ユーザーまたはグループを役割から削除する]。<li>`UserRemove`: ユーザーはアクティブな割り当てを無効にします。<li>`UserExtend`: ユーザーが期限切れの割り当てを拡張するよう要求します。</li><li>`AdminExtend`: 管理者は期限切れの割り当てを拡張します。</li><li>`UserRenew`: ユーザーは、期限切れの割り当ての更新を要求します。</li><li>`AdminRenew`: 管理者は期限切れの割り当てを拡張します。</li></ul>|
|割り当ての状態|String  |必須。 割り当ての状態を指定します。 値には、 <ul><li> `Eligible`適格な割り当ての場合</li><li> `Active`-管理者によって`Active`直接割り当てられている場合、またはユーザーによる資格のある割り当てでアクティブ化されている場合。</li></ul>|
|requesteddatetime          |DateTimeOffset |読み取り専用。 要求の作成時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|スケジューリング                   |[governanceSchedule](governanceschedule.md)|役割の割り当て要求の schedule オブジェクト。|
|したがっ                     |String         |必要な理由についての要求を作成するときに、ユーザーと管理者によって提供されるメッセージ。|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |役割の割り当て要求の状態。|
|linkedEligibleRoleAssignmentId|String        |これが役割のアクティブ化要求である場合は、参照`eligible assignment`されているの id を表します。それ以外の場合、 `null`値はです。 |



## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型                                |説明|
|:-------------|:----------------------------------|:----------|
|リソース      |[governanceResource](../resources/governanceresource.md)            |読み取り専用。 要求が目的とするリソース。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|読み取り専用。 要求が目的としているロール定義。 |
|subject       |[governanceSubject](../resources/governancesubject.md)|読み取り専用。 ユーザー/グループプリンシパル。|

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
