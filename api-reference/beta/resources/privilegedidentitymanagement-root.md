---
title: Azure AD Privileged Identity Management
description: Privileged Identity Management サービスで提供されているメソッドに一覧を示します。
localization_priority: Priority
ms.openlocfilehash: e5454a976a8dcdb17fea5ef9c217fc2eec9e2670
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344284"
---
# <a name="azure-ad-privileged-identity-management"></a>Azure AD Privileged Identity Management

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Privileged Identity Management](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-privileged-identity-management-configure/) サービスで提供されているメソッドに一覧を示します。

サービスは、OData 上にビルドされています。 クエリ結果をフィルター処理するには、URI で標準の OData ``$filter`` 式を使用します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[privilegedOperationEvent を一覧表示する](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md) コレクション |privilegedOperationEvent オブジェクト コレクションを取得します。 |
|[privilegedRole を取得する](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| privilegedRole オブジェクトを取得します。|
|[privilegedRole を一覧表示する](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) コレクション |privilegedRole オブジェクト コレクションを取得します。 |
|[ロールの割り当てを一覧表示する](../api/privilegedrole-list-assignments.md) | [privilegedRoleAssignment](privilegedroleassignment.md) コレクション |特定のロールの privilegedRoleAssignment コレクションを取得します。 各 privilegedRoleAssignment はユーザーに対するロールの割り当てを表します。|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |リクエスターに割り当てられているロールをアクティブ化します。|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |リクエスターに割り当てられているロールを非アクティブ化します。|
|[privilegedRoleAssignment を作成する](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| privilegedRoleAssignments コレクションを post して新しい privilegedRoleAssignment (ロールの割り当て) を作成します。|
|[privilegedRoleAssignment を一覧表示する](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) コレクション |privilegedRoleAssignment オブジェクト コレクションを取得します。 コレクションには、組織のすべてのロールの割り当てが含まれます。 各 privilegedRoleAssignment はユーザーに対するロールの割り当てを表します。 |
|[privilegedRoleAssignment を取得する](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|指定した割り当て ID の privilegedRoleAssignment オブジェクトを取得します。 |
|[privilegedRoleAssignment を削除する](../api/privilegedroleassignment-delete.md) | なし。 |privilegedRoleAssignment オブジェクトを削除します。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |ロールの割り当てを永続的にします。 |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |ロールの割り当てを有効にします。 |
|[my](../api/privilegedroleassignment-my.md) | [privilegedRoleAssignment](privilegedroleassignment.md) コレクション|リクエスターのロールの割り当てを取得します。 |
|[privilegedRoleSettings を取得する](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|privilegedRoleSettings オブジェクトのプロパティを取得します。 |
|[privilegedRoleSummary を取得する](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|privilegedRoleSummary オブジェクトを取得します。 |
|[privilegedApproval を取得する](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| privilegedApproval オブジェクトを取得します。|
|[privilegedApproval を一覧表示する](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md) コレクション |privilegedApproval オブジェクト コレクションを取得します。 |
|[privilegedApproval を作成する](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |privilegedApproval オブジェクトを作成します。 |
|[privilegedApproval を更新する](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |privilegedApproval オブジェクトを更新します。 |
|[myrequests](../api/privilegedapproval-myrequests.md) | [privilegedApproval](privilegedapproval.md) コレクション|リクエスターの承認要求を取得します。 |

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
