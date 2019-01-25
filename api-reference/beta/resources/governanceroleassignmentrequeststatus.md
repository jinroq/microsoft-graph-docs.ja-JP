---
title: governanceRoleAssignmentRequestStatus リソースの種類
description: GovernanceRoleAssignmentRequest の状態を表します。
localization_priority: Normal
ms.openlocfilehash: f4f0b23cf13de5beedb1964484ec4fbbb6e98720
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510177"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の状態を表します。


## <a name="properties"></a>プロパティ
プロパティ       | 型 |説明|
|:----|:-------------|:-----|
|status |String| 役割の割り当て要求のステータス。 値は、`InProgress`または`Closed`。|
|副状態 |String| 役割の割り当て要求のサブ状態です。 値は、 `Accepted`、 `PendingEvaluation`、 `Granted`、 `Denied`、 `PendingProvisioning`、 `Provisioned`、 `PendingRevocation`、 `Revoked`、 `Canceled`、 `Failed`、 `PendingApprovalProvisioning`、 `PendingApproval`、 `FailedAsResourceIsLocked`、 `PendingAdminDecision`、 `AdminApproved`、 `AdminDenied`、`TimedOut`と`ProvisioningStarted`。|
|statusDetails       |[keyValue](../resources/keyvalue.md)コレクション| 役割の割り当て要求の状態の詳細。 別のルールの評価の結果を表します。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyvalue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequeststatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
