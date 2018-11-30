---
title: educationClass リソース タイプ
description: '学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  '
ms.openlocfilehash: 4d61ca209b61b8b2b65fbe92b7ba16854e11fb37
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022867"
---
# <a name="educationclass-resource-type"></a>educationClass リソース タイプ

学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get educationClass](../api/educationclass-get.md) | [educationClass](educationclass.md) |**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Add member](../api/educationclass-post-members.md) |[educationUser](educationuser.md)| members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。|
|[List members](../api/educationclass-list-members.md) |[educationUser](educationuser.md) コレクション| **educationUser** オブジェクト コレクションを取得します。|
|[Remove student](../api/educationclass-delete-members.md) |[educationUser](educationuser.md)| members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。|
|[List schools](../api/educationclass-list-schools.md) |[educationSchool](educationschool.md) コレクション| **educationSchool** オブジェクト コレクションを取得します。|
|[Add teacher](../api/educationclass-post-teachers.md) |[educationUser](educationuser.md)| teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。|
|[List teachers](../api/educationclass-list-teachers.md) |[educationUser](educationuser.md) コレクション| クラスの教師一覧を取得します。|
|[Remove teacher](../api/educationclass-delete-teachers.md) |[educationUser](educationuser.md)| teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。|
|[Get group](../api/educationclass-get-group.md) |[group](group.md)| この **educationClass** に対応する Office 365 **group**を取得します。|
|[Update](../api/educationclass-update.md) | [educationClass](educationclass.md)    |**educationClass** オブジェクトを更新します。 |
|[Delete](../api/educationclass-delete.md) | なし |**educationClass** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id| String| クラスの一意の識別子。|
|説明|String| クラスの説明。|
|displayName|String| クラスの名前。|
|mailNickname|String| すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。 |
|createdBy|[identitySet](identityset.md)| クラスを作成したエンティティ。 |
|classCode|String| クラスを識別するために学校が使用するクラス コード。|
|externalId|String| 同期システムからのクラスの ID。 |
|externalName|String|同期システムからのクラスの名前。|
|externalSource|educationExternalSource| このクラスの作成方法。 可能な値: `sis`、 `manual`、 `unknownFutureValue`。|
|term|[educationTerm](educationterm.md)|このクラスの学期。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|members|[educationUser](../resources/educationuser.md) コレクション| クラスのすべてのユーザー。 Null 許容型。|
|schools|[educationSchool](../resources/educationschool.md) コレクション| このクラスに関連付けられているすべての学校。 Null 許容型。|
|teachers|[educationUser](../resources/educationuser.md) コレクション|  このクラスのすべての教師。 Null 許容型。|
|group|[group](../resources/group.md)| このクラスに対応するディレクトリのグループです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
