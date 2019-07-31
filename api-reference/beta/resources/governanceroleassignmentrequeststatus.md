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
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="6f06e-103">governanceRoleAssignmentRequestStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f06e-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f06e-104">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="6f06e-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="6f06e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f06e-105">Properties</span></span>
<span data-ttu-id="6f06e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f06e-106">Property</span></span>       | <span data-ttu-id="6f06e-107">型</span><span class="sxs-lookup"><span data-stu-id="6f06e-107">Type</span></span> |<span data-ttu-id="6f06e-108">説明</span><span class="sxs-lookup"><span data-stu-id="6f06e-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="6f06e-109">status</span><span class="sxs-lookup"><span data-stu-id="6f06e-109">status</span></span> |<span data-ttu-id="6f06e-110">String</span><span class="sxs-lookup"><span data-stu-id="6f06e-110">String</span></span>| <span data-ttu-id="6f06e-111">役割の割り当て要求の状態。</span><span class="sxs-lookup"><span data-stu-id="6f06e-111">The status of the role assignment request.</span></span> <span data-ttu-id="6f06e-112">値には、 `InProgress`また`Closed`はを指定できます。</span><span class="sxs-lookup"><span data-stu-id="6f06e-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="6f06e-113">サブ</span><span class="sxs-lookup"><span data-stu-id="6f06e-113">subStatus</span></span> |<span data-ttu-id="6f06e-114">String</span><span class="sxs-lookup"><span data-stu-id="6f06e-114">String</span></span>| <span data-ttu-id="6f06e-115">役割の割り当て要求のサブ状態。</span><span class="sxs-lookup"><span data-stu-id="6f06e-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="6f06e-116">値には、 `Accepted`、 `PendingEvaluation`、 `Granted`、 `Denied`、 `PendingProvisioning`、 `Provisioned`、 `PendingRevocation`、 `Revoked`、 `Canceled`、 `Failed`、 `PendingApprovalProvisioning`、 `PendingApproval`、 `FailedAsResourceIsLocked`、 `PendingAdminDecision`、、、 `TimedOut`、、 `ProvisioningStarted`の各値を指定`AdminApproved` `AdminDenied`できます。</span><span class="sxs-lookup"><span data-stu-id="6f06e-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="6f06e-117">statusDetails</span><span class="sxs-lookup"><span data-stu-id="6f06e-117">statusDetails</span></span>       |<span data-ttu-id="6f06e-118">[keyvalue](../resources/keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6f06e-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="6f06e-119">役割の割り当て要求の状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="6f06e-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="6f06e-120">さまざまなルールの評価結果を表します。</span><span class="sxs-lookup"><span data-stu-id="6f06e-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f06e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f06e-121">JSON representation</span></span>

<span data-ttu-id="6f06e-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6f06e-122">Here is a JSON representation of the resource.</span></span>

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
