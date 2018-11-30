---
title: Azure AD 特権 Id の管理
description: ここでは、管理者の Id 管理サービスによって提供されているメソッドの一覧です。
ms.openlocfilehash: ec060c4dc233677f1333e9588e4fb888f8dff9a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066269"
---
# <a name="azure-ad-privileged-identity-management"></a>Azure AD 特権 Id の管理

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ここでは、[管理者の Id 管理](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/)サービスによって提供されているメソッドの一覧です。

サービスは、OData の上に作成されます。 クエリの結果をフィルターするには、標準の OData を使用して、 ``$filter`` 、Uri で表現します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リスト privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md)コレクション |PrivilegedOperationEvent オブジェクトのコレクションを取得します。 |
|[PrivilegedRole を取得します。](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| PrivilegedRole オブジェクトを取得します。|
|[リスト privilegedRole](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md)コレクション |PrivilegedRole オブジェクトのコレクションを取得します。 |
|[リストのロールの割り当て](../api/privilegedrole-list-assignments.md) | [privilegedRoleAssignment](privilegedroleassignment.md)コレクション |特定のロールの privilegedRoleAssignment コレクションを取得します。 各 privilegedRoleAssignment は、ユーザーに役割の割り当てを表します。|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |リクエスターに割り当てられているロールをアクティブにします。|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |リクエスターに割り当てられているロールを非アクティブ化します。|
|[PrivilegedRoleAssignment を作成します。](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| PrivilegedRoleAssignments コレクションへの投稿には、新しい privilegedRoleAssignment (ロールの割り当て) を作成します。|
|[リスト privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md)コレクション |PrivilegedRoleAssignment オブジェクトのコレクションを取得します。 コレクションには、組織のすべてのロールの割り当てが含まれています。 各 privilegedRoleAssignment は、ユーザーに役割の割り当てを表します。 |
|[PrivilegedRoleAssignment を取得します。](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|指定した割り当ての id を持つ privilegedRoleAssignment オブジェクトを取得します。 |
|[PrivilegedRoleAssignment を削除します。](../api/privilegedroleassignment-delete.md) | なし。 |PrivilegedRoleAssignment オブジェクトを削除します。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |として永続的な役割の割り当てを確認します。 |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |対象となるように、役割の割り当てを確認します。 |
|[私の](../api/privilegedroleassignment-my.md) | [privilegedRoleAssignment](privilegedroleassignment.md)コレクション|要求側のロールの割り当てを取得します。 |
|[PrivilegedRoleSettings を取得します。](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|PrivilegedRoleSettings オブジェクトのプロパティを取得します。 |
|[PrivilegedRoleSummary を取得します。](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|PrivilegedRoleSummary オブジェクトを取得します。 |
|[PrivilegedApproval を取得します。](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| PrivilegedApproval オブジェクトを取得します。|
|[リスト privilegedApproval](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md)コレクション |PrivilegedApproval オブジェクトのコレクションを取得します。 |
|[PrivilegedApproval を作成します。](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |PrivilegedApproval オブジェクトを作成します。 |
|[PrivilegedApproval を更新します。](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |PrivilegedApproval オブジェクトを更新します。 |
|[myrequests](../api/privilegedapproval-myrequests.md) | [privilegedApproval](privilegedapproval.md)コレクション|要求側の承認の要求を取得します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
