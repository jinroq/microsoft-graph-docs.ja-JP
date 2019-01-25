---
title: privilegedRoleAssignment リソースの種類
description: '特定のユーザーに対して権限を持つ役割の割り当てを表します。 '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515119"
---
# <a name="privilegedroleassignment-resource-type"></a>privilegedRoleAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定のユーザーに対して権限を持つ役割の割り当てを表します。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[PrivilegedRoleAssignment コレクションのリスト](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md)コレクション|PrivilegedRoleAssignment オブジェクトのコレクションを取得します。|
|[PrivilegedRoleAssignment を取得します。](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |PrivilegedRoleAssignment オブジェクトのプロパティと関係を参照してください。|
|[割り当てを作成します。](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| 割り当てのコレクションへの投稿には、新しい割り当てを作成します。|
|[Delete](../api/privilegedroleassignment-delete.md) | なし |PrivilegedRoleAssignment オブジェクトを削除します。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|として永続的な役割の割り当てを確認します。|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|対象となるように、役割の割り当てを確認します。|
|[My](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md)コレクション|現在のユーザーの特権を持つ役割の割り当てを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|一時的な特権を持つロールの割り当ては期限が切れた場合は、UTC 日時です。 永続的な役割の割り当ての値が null です。|
|id|string| 特権を持つ役割の割り当ての一意の識別子です。 読み取り専用です。 'UserId_roleId'、Azure AD ユーザーの id の GUID の文字列は、ユーザー Id、roleId は、Azure の管理者ロールの id の GUID の文字列の形式であります。|
|isElevated|boolean|**true の**ロールの割り当てが有効な場合です。 **false**役割の割り当てが無効になった場合。|
|resultMessage|string|結果のメッセージがサービスによって設定されます。|
|roleId|string|ロール識別子 GUID の文字列形式。|
|userId|string|ユーザーの識別子です。 GUID の文字列形式。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| 読み取り専用です。 Null 許容型。 関連付けられているロールの情報です。|

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
