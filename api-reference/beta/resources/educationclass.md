---
title: educationClass リソース タイプ
description: 学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0bc9fa375e3f22087fbf268933370d8a6222654e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006368"
---
# <a name="educationclass-resource-type"></a>educationClass リソース タイプ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office 365 エクスペリエンスが正常に機能するには、教師が教師コレクションと members コレクションの両方のメンバーである必要があります。

## <a name="methods"></a>メソッド

| メソッド                                                                  | 戻り値の型                                    | 説明                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [Get educationClass](../api/educationclass-get.md)                      | [educationClass]                               | **educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。                        |
| [Add member](../api/educationclass-post-members.md)                     | [educationUser]                                | members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。  |
| [List members](../api/educationclass-list-members.md)                   | [educationUser] コレクション                     | **educationUser** オブジェクト コレクションを取得します。                                               |
| [Remove student](../api/educationclass-delete-members.md)               | [educationUser]                                | members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。       |
| [List schools](../api/educationclass-list-schools.md)                   | [educationSchool] コレクション                   | **educationSchool** オブジェクト コレクションを取得します。                                             |
| [Add teacher](../api/educationclass-post-teachers.md)                   | [educationUser]                                | teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。 |
| [List teachers](../api/educationclass-list-teachers.md)                 | [educationUser] コレクション                     | クラスの教師一覧を取得します。                                                     |
| [Remove teacher](../api/educationclass-delete-teachers.md)              | [educationUser]                                | teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。      |
| [EducationAssignment を作成する](../api/educationclass-post-assignments.md) | [educationAssignment]                          | Assignments コレクションへの投稿によって新しい**educationAssignment**を作成します。            |
| [割り当てを一覧表示する](../api/educationclass-list-assignments.md)           | [educationAssignment]コレクション                | **EducationAssignment**オブジェクトのコレクションを取得します。                                         |
| [グループを取得する](../api/educationclass-get-group.md)                         | [group]                                        | この **educationClass** に対応する Office 365 **group**を取得します。                 |
| [EducationCategory を作成する](../api/educationclass-post-category.md)      | [educationCategory]                            | このクラスの新しい**educationCategory**を作成します。                                        |
| [カテゴリの一覧表示](../api/educationclass-list-categories.md)             | [educationCategory]コレクション                 | このクラスに属する**educationCategory**オブジェクトのリストを取得します。                      |
| [Update](../api/educationclass-update.md)                               | [educationClass]                               | **educationClass** オブジェクトを更新します。                                                         |
| [Delete](../api/educationclass-delete.md)                               | None                                           | **educationClass** オブジェクトを削除します。                                                         |
| [差分](../api/educationclass-delta.md)                                 | [educationClass](educationclass.md) コレクション | **EducationClasses**の増分の変更を取得する                                          |

## <a name="properties"></a>プロパティ

| プロパティ       | 型                                  | 説明                                                                             |
| :------------- | :------------------------------------ | :-------------------------------------------------------------------------------------- |
| id             | 文字列                                | クラスの一意の識別子。                                                        |
| classCode      | String                                | クラスを識別するために学校が使用するクラス コード。                                    |
| 学習         | [educationCourse](educationcourse.md) | クラスのコース情報                                                        |
| createdBy      | [identitySet]                         | クラスを作成したエンティティ。                                                            |
| description    | String                                | クラスの説明。                                                               |
| displayName    | 文字列                                | クラスの名前。                                                                      |
| externalId     | String                                | 同期システムからのクラスの ID。                                                |
| externalName   | String                                | 同期システムからのクラスの名前。                                                |
| externalSource | string                                | このクラスの作成方法。 使用可能な値: `sis`、`manual`、`unknownFutureValue`。 |
| mailNickname   | String                                | すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。                         |
| term           | [educationTerm]                       | クラスの用語。                                                                     |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                             | 説明                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| assignments  | [educationAssignment]コレクション | このクラスに関連付けられているすべての割り当て。 Null 許容型。     |
| members      | [educationUser] コレクション       | クラスのすべてのユーザー。 Null 許容型。                         |
| schools      | [educationSchool] コレクション     | このクラスに関連付けられているすべての学校。 Null 許容型。 |
| teachers     | [educationUser] コレクション       | このクラスのすべての教師。 Null 許容型。                      |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "classCode": "String",
  "course": { "@odata.type": "microsoft.graph.educationCourse" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "id": "String (identifier)",
  "mailNickname": "String",
  "term": { "@odata.type": "microsoft.graph.educationTerm" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.educationClass",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationClass has documented navigation properties, but we thought it was a complex type!",
    "Resource educationClass has documented navigation properties, but we thought it was a complex type!"
  ]

}-->

[educationclass]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[educationcategory]: educationcategory.md
[educationschool]: educationschool.md
[educationterm]: educationterm.md
[identityset]: identityset.md
[group]: group.md
