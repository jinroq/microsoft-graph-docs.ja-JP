---
title: educationClass リソース タイプ
description: '学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f651e695ddf0b7139a31d077dcf021fced91293a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962920"
---
# <a name="educationclass-resource-type"></a>educationClass リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
|[EducationAssignment を作成します。](../api/educationclass-post-assignments.md) |[educationAssignment](../resources/educationassignment.md)| 割り当てのコレクションへの投稿には、新しい**educationAssignment**を作成します。|
|[リストの割り当て](../api/educationclass-list-assignments.md) |[educationAssignment](../resources/educationassignment.md)コレクション| **EducationAssignment**オブジェクトのコレクションを取得します。|
|[グループを取得する](../api/educationclass-get-group.md) |[group](group.md)| この **educationClass** に対応する Office 365 **group**を取得します。|
|[Update](../api/educationclass-update.md) | [educationClass](educationclass.md)    |**educationClass** オブジェクトを更新します。 |
|[Delete](../api/educationclass-delete.md) | なし |**educationClass** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID| String| クラスの一意の識別子。|
|説明|String| クラスの説明。|
|displayName|String| クラスの名前。|
|mailNickname|String| すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。 |
|createdBy|[identitySet](identityset.md)| クラスを作成したエンティティ。 |
|classCode|String| クラスを識別するために学校が使用するクラス コード。|
|externalId|String| 同期システムからのクラスの ID。 |
|externalName|String|同期システムからのクラスの名前。|
|externalSource|文字列| このクラスの作成方法。 使用可能な値: `sis`、`manual`、`unknownFutureValue`。|
|term|[educationTerm](educationterm.md)|このクラスの学期。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|members|[educationUser](../resources/educationuser.md) コレクション| クラスのすべてのユーザー。 Null 許容型。|
|schools|[educationSchool](../resources/educationschool.md) コレクション| このクラスに関連付けられているすべての学校。 Null 許容型。|
|teachers|[educationUser](../resources/educationuser.md) コレクション|  このクラスのすべての教師。 Null 許容型。|
|assignments|[educationAssignment](../resources/educationassignment.md)コレクション| このクラスに関連付けられているすべての割り当て。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "term": {"@odata.type": "microsoft.graph.education.term"}
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
