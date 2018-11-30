---
title: privilegedRoleAssignment リソースの種類
description: '特定のユーザーに対して権限を持つ役割の割り当てを表します。 '
ms.openlocfilehash: 40cfe6487184171fc0d120f9a0e2cd98070f96f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068586"
---
# <a name="privilegedroleassignment-resource-type"></a>privilegedRoleAssignment リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特定のユーザーに対して権限を持つ役割の割り当てを表します。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[PrivilegedRoleAssignment コレクションのリスト](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md)コレクション|PrivilegedRoleAssignment オブジェクトのコレクションを取得します。|
|[PrivilegedRoleAssignment を取得します。](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |PrivilegedRoleAssignment オブジェクトのプロパティと関係を参照してください。|
|[割り当てを作成します。](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| 割り当てのコレクションへの投稿には、新しい割り当てを作成します。|
|[削除](../api/privilegedroleassignment-delete.md) | なし |PrivilegedRoleAssignment オブジェクトを削除します。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|として永続的な役割の割り当てを確認します。|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|対象となるように、役割の割り当てを確認します。|
|[私の](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md)コレクション|現在のユーザーの特権を持つ役割の割り当てを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|一時的な特権を持つロールの割り当ては期限が切れた場合は、UTC 日時です。 永続的な役割の割り当ての値が null です。|
|ID|文字列| 特権を持つ役割の割り当ての一意の識別子です。 読み取り専用。 'UserId_roleId'、Azure AD ユーザーの id の GUID の文字列は、ユーザー Id、roleId は、Azure の管理者ロールの id の GUID の文字列の形式であります。|
|isElevated|ブール|**true の**ロールの割り当てが有効な場合です。 **false**役割の割り当てが無効になった場合。|
|resultMessage|文字列|結果のメッセージがサービスによって設定されます。|
|roleId|文字列|ロールの識別子です。 GUID の文字列形式。|
|userId|文字列|ユーザーの識別子です。 GUID の文字列形式。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| 読み取り専用。 Null 許容型。 関連付けられているロールの情報です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->