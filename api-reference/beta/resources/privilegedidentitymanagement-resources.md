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
# <a name="privileged-identity-management---azure-resources"></a>Privileged Identity Management - Azure リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

管理グループ、サブスクリプション、リソース グループ、およびリソースのレベルで Azure のインフラストラクチャ役割に対応する Just-In-Time アクセスのワークフローを設定するために、 Azure リソースの [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) を使用できます。 これらには、カスタム RBAC ロールと同様に、所有者や共同作成者のロールなどの組み込みのロールが含まれます。

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a>REST API を使用した PIM および Azure リソースの一般的なユースケース

| ユースケース | リソース | 関連項目 |
| --- | --- | --- |
| PIM 管理のリソース (サブスクリプション、リソース グループ、リソースなど) の追加、アクセス権を持つすべての管理リソースの要求者の一覧表示、管理リソースの関係の取得を行います。 | [governanceResource](governanceresource.md) | [ロールの検出と管理](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| リソースのすべてのロールを一覧表示したり、指定したリソースから特定のロールの詳細を入手したりします。 | [governanceRoleDefinition](governanceroledefinition.md) |  |
| リソースに設定されているすべてのロールを取得したり、ロールの設定を更新したりします。 | [governanceRoleSetting](governancerolesetting.md) | [ロールの設定を構成する](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| リソースのすべてのロールの割り当ての一覧表示とエクスポートを行います。 | [governanceRoleAssignment](governanceroleassignment.md) | [ロールの割り当てをエクスポートする](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| 資格のあるまたはアクティブなロールの割り当ての作成または削除、資格のある割り当てのアクティブ化または非アクティブ化、保留中の要求の一覧表示、保留中の要求の承認または拒否あるいは自分の保留中の要求の取り消しを行います。 | [governanceRoleAssignmentRequest](governanceroleassignmentrequest.md) | [ロールの割り当て](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[ロールのアクティブ化](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[申請の承認](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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
