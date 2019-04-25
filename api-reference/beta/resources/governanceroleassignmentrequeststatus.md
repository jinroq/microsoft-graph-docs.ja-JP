---
title: governanceRoleAssignmentRequestStatus リソースの種類
description: governanceRoleAssignmentRequest の状態を表します。
localization_priority: Normal
ms.openlocfilehash: f4f0b23cf13de5beedb1964484ec4fbbb6e98720
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547433"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の状態を表します。


## <a name="properties"></a>プロパティ
プロパティ       | 型 |説明|
|:----|:-------------|:-----|
|status |String| 役割の割り当て要求の状態。 値には、 `InProgress`また`Closed`はを指定できます。|
|サブ |String| 役割の割り当て要求のサブ状態。 値には、 `Accepted`、 `PendingEvaluation`、 `Granted`、 `Denied`、 `PendingProvisioning`、 `Provisioned`、 `PendingRevocation`、 `Revoked`、 `Canceled`、 `Failed`、 `PendingApprovalProvisioning`、 `PendingApproval`、 `FailedAsResourceIsLocked`、 `PendingAdminDecision`、、、 `TimedOut`、、 `ProvisioningStarted`の各値を指定`AdminApproved` `AdminDenied`できます。|
|statusdetails       |[keyvalue](../resources/keyvalue.md) コレクション| 役割の割り当て要求の状態の詳細。 さまざまなルールの評価結果を表します。 |

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
