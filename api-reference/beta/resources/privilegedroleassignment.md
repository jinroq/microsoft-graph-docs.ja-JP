---
title: privilegedRoleAssignment リソースの種類
description: '特定のユーザーの特権の役割の割り当てを表します。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 010dbf110de414e5221873263ffb5bcffe30db48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008881"
---
# <a name="privilegedroleassignment-resource-type"></a>privilegedRoleAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定のユーザーの特権の役割の割り当てを表します。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[PrivilegedRoleAssignment コレクションを一覧表示する](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) コレクション|PrivilegedRoleAssignment オブジェクトのコレクションを取得します。|
|[privilegedRoleAssignment を取得する](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |PrivilegedRoleAssignment オブジェクトのプロパティとリレーションシップを読み取ります。|
|[割り当てを作成する](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Assignments コレクションに投稿して、新しい割り当てを作成します。|
|[Delete](../api/privilegedroleassignment-delete.md) | None |privilegedRoleAssignment オブジェクトを削除します。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|ロールの割り当てを永続的にします。|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|ロールの割り当てを有効にします。|
|[my](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md) コレクション|現在のユーザーの特権の役割の割り当てを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|一時的な特権の役割の割り当てが期限切れになる UTC の DateTime。 永続的な役割の割り当ての場合、値は null になります。|
|id|string| 特権の役割の割り当ての一意識別子。 読み取り専用です。 これは ' userId_roleId ' の形式になっています。ここで、userId は Azure AD ユーザー id の GUID 文字列で、roleId は Azure 管理者の役割 id の GUID 文字列です。|
|isElevated|ブール値|役割の割り当てがアクティブ化されている場合は**true** 。 **false**を指定すると、役割の割り当てが非アクティブになります。|
|resultMessage|string|サービスによって設定された結果メッセージ。|
|roleId|string|ロール識別子。 GUID 文字列形式。|
|userId|string|ユーザー識別子。 GUID 文字列形式。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| 読み取り専用です。 Null 許容型。 関連付けられているロール情報。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->
