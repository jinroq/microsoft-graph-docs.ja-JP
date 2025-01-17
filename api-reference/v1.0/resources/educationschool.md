---
title: educationSchool リソースの種類
description: '学校を表すリソースで、その学校のクラス、教師、学生を管理するために使用します。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3446b637835facfbe9a03e31dbdb8e9421b2faed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030507"
---
# <a name="educationschool-resource-type"></a>educationSchool リソースの種類

学校を表すリソースで、その学校のクラス、教師、学生を管理するために使用します。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get](../api/educationschool-get.md) | [educationSchool](educationschool.md) |**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Add class](../api/educationschool-post-classes.md) |[educationClass](educationclass.md)| classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。|
|[List classes](../api/educationschool-list-classes.md) |[educationClass](educationclass.md) コレクション| **educationClass** オブジェクト コレクションを取得します。|
|[Remove class](../api/educationschool-delete-classes.md) |[educationClass](educationclass.md)| classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。|
|[Add user](../api/educationschool-post-users.md) |[educationUser](educationuser.md)| **users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。|
|[List users](../api/educationschool-list-users.md) |[educationUser](educationuser.md) コレクション| **educationUser** オブジェクト コレクションを取得します。|
|[Remove user](../api/educationschool-delete-users.md) |[educationUser](educationuser.md)| **users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。|
|[Update](../api/educationschool-update.md) | [educationSchool](educationschool.md) |**educationSchool** オブジェクトを更新します。 |
|[Delete](../api/educationschool-delete.md) | None |**educationSchool** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|文字列|この学校の GUID。|
|displayName| 文字列| 学校の表示名。| 
|description| String | 学校の説明。| 
|status| string| 読み取り専用。 使用可能な値: `inactive`、`active`、`expired`、`deleteable`。|
|externalSource| educationExternalSource| 読み取り専用です。  使用可能な値: `sis`、`manual`、`unknownFutureValue`。|
|principalEmail| String| プリンシパルの電子メール アドレス。|
|principalName| String | プリンシパルの名前。|
|externalPrincipalId| String | 同期システム内のプリンシパルの ID。 |
|highestGrade|String| 授業を受けている最高学年。 |
|lowestGrade|String| 授業を受けている最低学年。 |
|schoolNumber|String| 学校番号。|
|externalId|String| 同期システム内の学校の ID。 |
|phone|String| 学校の電話番号。 |
|fax|String| 学校の FAX 番号。 |
|address|[physicalAddress](physicaladdress.md)| 学校の住所。|
|createdBy|[identitySet](identityset.md)|学校を作成したエンティティ。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) コレクション| 学校で授業しているクラス。 Null 許容型。|
|users|[educationUser](educationuser.md) コレクション| 学校のユーザー。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
