---
title: governanceRoleAssignmentRequestStatus リソースの種類
description: GovernanceRoleAssignmentRequest の状態を表します。
localization_priority: Normal
ms.openlocfilehash: c5daac53661cc607d51e5bfd1ec9031cfa599fca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808072"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の状態を表します。


## <a name="properties"></a>プロパティ
プロパティ       | 種類 |説明|
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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
