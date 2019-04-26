---
title: governanceRoleAssignmentRequestStatus リソースの種類
description: governanceRoleAssignmentRequest の状態を表します。
localization_priority: Normal
ms.openlocfilehash: 768ef092dbe52b0989277905bae03eee091ca8c6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340322"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="e597e-103">governanceRoleAssignmentRequestStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e597e-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e597e-104">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="e597e-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="e597e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e597e-105">Properties</span></span>
<span data-ttu-id="e597e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e597e-106">Property</span></span>       | <span data-ttu-id="e597e-107">型</span><span class="sxs-lookup"><span data-stu-id="e597e-107">Type</span></span> |<span data-ttu-id="e597e-108">説明</span><span class="sxs-lookup"><span data-stu-id="e597e-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="e597e-109">status</span><span class="sxs-lookup"><span data-stu-id="e597e-109">status</span></span> |<span data-ttu-id="e597e-110">String</span><span class="sxs-lookup"><span data-stu-id="e597e-110">String</span></span>| <span data-ttu-id="e597e-111">役割の割り当て要求の状態。</span><span class="sxs-lookup"><span data-stu-id="e597e-111">The status of the role assignment request.</span></span> <span data-ttu-id="e597e-112">値には、 `InProgress`また`Closed`はを指定できます。</span><span class="sxs-lookup"><span data-stu-id="e597e-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="e597e-113">サブ</span><span class="sxs-lookup"><span data-stu-id="e597e-113">subStatus</span></span> |<span data-ttu-id="e597e-114">String</span><span class="sxs-lookup"><span data-stu-id="e597e-114">String</span></span>| <span data-ttu-id="e597e-115">役割の割り当て要求のサブ状態。</span><span class="sxs-lookup"><span data-stu-id="e597e-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="e597e-116">値には、 `Accepted`、 `PendingEvaluation`、 `Granted`、 `Denied`、 `PendingProvisioning`、 `Provisioned`、 `PendingRevocation`、 `Revoked`、 `Canceled`、 `Failed`、 `PendingApprovalProvisioning`、 `PendingApproval`、 `FailedAsResourceIsLocked`、 `PendingAdminDecision`、、、 `TimedOut`、、 `ProvisioningStarted`の各値を指定`AdminApproved` `AdminDenied`できます。</span><span class="sxs-lookup"><span data-stu-id="e597e-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="e597e-117">statusdetails</span><span class="sxs-lookup"><span data-stu-id="e597e-117">statusDetails</span></span>       |<span data-ttu-id="e597e-118">[keyvalue](../resources/keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e597e-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="e597e-119">役割の割り当て要求の状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="e597e-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="e597e-120">さまざまなルールの評価結果を表します。</span><span class="sxs-lookup"><span data-stu-id="e597e-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e597e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e597e-121">JSON representation</span></span>

<span data-ttu-id="e597e-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e597e-122">Here is a JSON representation of the resource.</span></span>

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
