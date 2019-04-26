---
title: privilegedRoleAssignment リソースの種類
description: '特定のユーザーの特権の役割の割り当てを表します。 '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563425"
---
# <a name="privilegedroleassignment-resource-type"></a>privilegedRoleAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定のユーザーの特権の役割の割り当てを表します。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[privilegedRoleAssignment コレクションを一覧表示する](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md)コレクション|privilegedRoleAssignment オブジェクトのコレクションを取得します。|
|[privilegedRoleAssignment を取得する](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |privilegedRoleAssignment オブジェクトのプロパティとリレーションシップを読み取ります。|
|[割り当てを作成する](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| assignments コレクションに投稿して、新しい割り当てを作成します。|
|[削除](../api/privilegedroleassignment-delete.md) | なし |privilegedRoleAssignment オブジェクトを削除します。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|役割の割り当てを永続的に設定します。|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|役割の割り当てを対象として設定します。|
|[私の](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md)コレクション|現在のユーザーの特権の役割の割り当てを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|一時的な特権の役割の割り当てが期限切れになる UTC の DateTime。 永続的な役割の割り当ての場合、値は null になります。|
|id|string| 特権の役割の割り当ての一意識別子。 読み取り専用。 これは ' userId_roleId ' の形式になっています。ここで、userId は azure AD ユーザー id の guid 文字列で、roleId は azure 管理者の役割 id の guid 文字列です。|
|isElevated|ブール値|役割の割り当てがアクティブ化されている場合は**true** 。 **false**を指定すると、役割の割り当てが非アクティブになります。|
|resultmessage|string|サービスによって設定された結果メッセージ。|
|roleId|string|ロール識別子。 GUID 文字列形式。|
|userId|string|ユーザー識別子。 GUID 文字列形式。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|roleinfo|[privilegedRole](privilegedrole.md)| 読み取り専用。 Null 許容型。 関連付けられているロール情報。|

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
