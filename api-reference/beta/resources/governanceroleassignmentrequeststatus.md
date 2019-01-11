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
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="70fc5-103">governanceRoleAssignmentRequestStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70fc5-103">governanceRoleAssignmentRequestStatus resource type</span></span>

> <span data-ttu-id="70fc5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="70fc5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70fc5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70fc5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70fc5-106">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="70fc5-106">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="70fc5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70fc5-107">Properties</span></span>
<span data-ttu-id="70fc5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70fc5-108">Property</span></span>       | <span data-ttu-id="70fc5-109">種類</span><span class="sxs-lookup"><span data-stu-id="70fc5-109">Type</span></span> |<span data-ttu-id="70fc5-110">説明</span><span class="sxs-lookup"><span data-stu-id="70fc5-110">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="70fc5-111">status</span><span class="sxs-lookup"><span data-stu-id="70fc5-111">status</span></span> |<span data-ttu-id="70fc5-112">String</span><span class="sxs-lookup"><span data-stu-id="70fc5-112">String</span></span>| <span data-ttu-id="70fc5-113">役割の割り当て要求のステータス。</span><span class="sxs-lookup"><span data-stu-id="70fc5-113">The status of the role assignment request.</span></span> <span data-ttu-id="70fc5-114">値は、`InProgress`または`Closed`。</span><span class="sxs-lookup"><span data-stu-id="70fc5-114">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="70fc5-115">副状態</span><span class="sxs-lookup"><span data-stu-id="70fc5-115">subStatus</span></span> |<span data-ttu-id="70fc5-116">String</span><span class="sxs-lookup"><span data-stu-id="70fc5-116">String</span></span>| <span data-ttu-id="70fc5-117">役割の割り当て要求のサブ状態です。</span><span class="sxs-lookup"><span data-stu-id="70fc5-117">The sub status of the role assignment request.</span></span> <span data-ttu-id="70fc5-118">値は、 `Accepted`、 `PendingEvaluation`、 `Granted`、 `Denied`、 `PendingProvisioning`、 `Provisioned`、 `PendingRevocation`、 `Revoked`、 `Canceled`、 `Failed`、 `PendingApprovalProvisioning`、 `PendingApproval`、 `FailedAsResourceIsLocked`、 `PendingAdminDecision`、 `AdminApproved`、 `AdminDenied`、`TimedOut`と`ProvisioningStarted`。</span><span class="sxs-lookup"><span data-stu-id="70fc5-118">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="70fc5-119">statusDetails</span><span class="sxs-lookup"><span data-stu-id="70fc5-119">statusDetails</span></span>       |<span data-ttu-id="70fc5-120">[keyValue](../resources/keyvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="70fc5-120">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="70fc5-121">役割の割り当て要求の状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="70fc5-121">The details of the status of the role assignment request.</span></span> <span data-ttu-id="70fc5-122">別のルールの評価の結果を表します。</span><span class="sxs-lookup"><span data-stu-id="70fc5-122">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70fc5-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70fc5-123">JSON representation</span></span>

<span data-ttu-id="70fc5-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="70fc5-124">Here is a JSON representation of the resource.</span></span>

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
