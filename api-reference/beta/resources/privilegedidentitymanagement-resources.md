---
title: Privileged Identity Management - Azure リソース
description: Azure AD Privileged Identity Management の API で Azure リソースを管理します。
localization_priority: Priority
ms.openlocfilehash: b4b6a85e92784c14f95003e2e6d7d18ebde89b74
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2019
ms.locfileid: "34425146"
---
# <a name="privileged-identity-management---azure-resources"></a><span data-ttu-id="e1990-103">Privileged Identity Management - Azure リソース</span><span class="sxs-lookup"><span data-stu-id="e1990-103">Privileged Identity Management - Azure resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1990-104">管理グループ、サブスクリプション、リソース グループ、およびリソースのレベルで Azure のインフラストラクチャ役割に対応する Just-In-Time アクセスのワークフローを設定するために、 Azure リソースの [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="e1990-104">You can use [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) for Azure resources to set up just-in-time access workflow for your Azure infrastructure roles at a management group, subscription, resource group, and resource level.</span></span> <span data-ttu-id="e1990-105">これらには、カスタム RBAC ロールと同様に、所有者や共同作成者のロールなどの組み込みのロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e1990-105">These include built-in roles like Owner and Contributor as well as custom RBAC roles.</span></span>

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a><span data-ttu-id="e1990-106">REST API を使用した PIM および Azure リソースの一般的なユースケース</span><span class="sxs-lookup"><span data-stu-id="e1990-106">Common use cases for PIM and Azure resources using a REST API</span></span>

| <span data-ttu-id="e1990-107">ユースケース</span><span class="sxs-lookup"><span data-stu-id="e1990-107">Use case</span></span> | <span data-ttu-id="e1990-108">リソース</span><span class="sxs-lookup"><span data-stu-id="e1990-108">Resource</span></span> | <span data-ttu-id="e1990-109">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1990-109">See also</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e1990-110">PIM 管理のリソース (サブスクリプション、リソース グループ、リソースなど) の追加、アクセス権を持つすべての管理リソースの要求者の一覧表示、管理リソースの関係の取得を行います。</span><span class="sxs-lookup"><span data-stu-id="e1990-110">Onboard a resource (subscriptions, resource group, resource etc.) for PIM management, list all the managed resources requester have access to, and retrieve relationships of a managed resource.</span></span> | [<span data-ttu-id="e1990-111">governanceResource</span><span class="sxs-lookup"><span data-stu-id="e1990-111">governanceResource</span></span>](governanceresource.md) | [<span data-ttu-id="e1990-112">ロールの検出と管理</span><span class="sxs-lookup"><span data-stu-id="e1990-112">Role discovery and management</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| <span data-ttu-id="e1990-113">リソースのすべてのロールを一覧表示したり、指定したリソースから特定のロールの詳細を入手したりします。</span><span class="sxs-lookup"><span data-stu-id="e1990-113">List all the roles for a resource or get details of a particular role in a specified resource.</span></span> | [<span data-ttu-id="e1990-114">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e1990-114">governanceRoleDefinition</span></span>](governanceroledefinition.md) |  |
| <span data-ttu-id="e1990-115">リソースに設定されているすべてのロールを取得したり、ロールの設定を更新したりします。</span><span class="sxs-lookup"><span data-stu-id="e1990-115">Retrieve all role settings for a resource or make an update to a role setting</span></span> | [<span data-ttu-id="e1990-116">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="e1990-116">governanceRoleSetting</span></span>](governancerolesetting.md) | [<span data-ttu-id="e1990-117">ロールの設定を構成する</span><span class="sxs-lookup"><span data-stu-id="e1990-117">Configure role setting</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| <span data-ttu-id="e1990-118">リソースのすべてのロールの割り当ての一覧表示とエクスポートを行います。</span><span class="sxs-lookup"><span data-stu-id="e1990-118">List and export all role assignments for a resource.</span></span> | [<span data-ttu-id="e1990-119">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e1990-119">governanceRoleAssignment</span></span>](governanceroleassignment.md) | [<span data-ttu-id="e1990-120">ロールの割り当てをエクスポートする</span><span class="sxs-lookup"><span data-stu-id="e1990-120">Export role assignments</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| <span data-ttu-id="e1990-121">資格のあるまたはアクティブなロールの割り当ての作成または削除、資格のある割り当てのアクティブ化または非アクティブ化、保留中の要求の一覧表示、保留中の要求の承認または拒否あるいは自分の保留中の要求の取り消しを行います。</span><span class="sxs-lookup"><span data-stu-id="e1990-121">Create or remove an eligible or active role assignment, activate/deactivate an eligible assignment, view a list of pending requests, approve or deny a pending request or cancel your own pending request.</span></span> | [<span data-ttu-id="e1990-122">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e1990-122">governanceRoleAssignmentRequest</span></span>](governanceroleassignmentrequest.md) | [<span data-ttu-id="e1990-123">ロールの割り当て</span><span class="sxs-lookup"><span data-stu-id="e1990-123">Role assignment</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[<span data-ttu-id="e1990-124">ロールのアクティブ化</span><span class="sxs-lookup"><span data-stu-id="e1990-124">Role activation</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[<span data-ttu-id="e1990-125">申請の承認</span><span class="sxs-lookup"><span data-stu-id="e1990-125">Approve or deny requests</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->