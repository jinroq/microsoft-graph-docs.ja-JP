---
title: governanceRoleAssignmentRequestStatus リソースの種類
description: GovernanceRoleAssignmentRequest の状態を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ca61e5e3ef5456889eafcef3914f16fc072dfb6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971865"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の状態を表します。


## <a name="properties"></a>プロパティ
プロパティ       | 型 |説明|
|:----|:-------------|:-----|
|status |String| 役割の割り当て要求の状態。 値には、 `InProgress`また`Closed`はを指定できます。|
|サブ |String| 役割の割り当て要求のサブ状態。 値には、 `Accepted`、 `PendingEvaluation`、 `Granted`、 `Denied`、 `PendingProvisioning`、 `Provisioned`、 `PendingRevocation`、 `Revoked`、 `Canceled`、 `Failed`、 `PendingApprovalProvisioning`、 `PendingApproval`、 `FailedAsResourceIsLocked`、 `PendingAdminDecision`、、、 `TimedOut`、、 `ProvisioningStarted`の各値を指定`AdminApproved` `AdminDenied`できます。|
|statusDetails       |[keyvalue](../resources/keyvalue.md) コレクション| 役割の割り当て要求の状態の詳細。 さまざまなルールの評価結果を表します。 |

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
  "statusDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
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
  "suppressions": []
}
-->
