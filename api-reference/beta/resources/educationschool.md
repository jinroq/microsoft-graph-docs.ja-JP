---
title: educationSchool リソースの種類
description: '学校。 **EducationSchool**リソースは現在、administrativeUnit リソースに対応しており、同じ ID を共有しています。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9cded9db9ab9d7310a10ab690e05f49dca8711c8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750144"
---
# <a name="educationschool-resource-type"></a>educationSchool リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校。 **EducationSchool**リソースは現在、 [administrativeUnit](administrativeunit.md)リソースに対応しており、同じ ID を共有しています。

このリソースは[educationOrganization](educationorganization.md)のサブタイプです。

## <a name="methods"></a>メソッド

| メソッド                                                                     | 戻り値の型                                      | 説明                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [Get](../api/educationschool-get.md)                                       | [educationSchool](educationschool.md)            | **educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。                         |
| [Add class](../api/educationschool-post-classes.md)                        | [educationClass](educationclass.md)              | classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。  |
| [List classes](../api/educationschool-list-classes.md)                     | [educationClass](educationclass.md) コレクション   | **educationClass** オブジェクト コレクションを取得します。                                               |
| [Remove class](../api/educationschool-delete-classes.md)                   | [educationClass](educationclass.md)              | classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。       |
| [Add user](../api/educationschool-post-users.md)                           | [educationUser](educationuser.md)                | **users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。 |
| [List users](../api/educationschool-list-users.md)                         | [educationUser](educationuser.md) コレクション     | **educationUser** オブジェクト コレクションを取得します。                                                |
| [Remove user](../api/educationschool-delete-users.md)                      | [educationUser](educationuser.md)                | **users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。      |
| [AdministrativeUnit を取得する](../api/educationschool-get-administrativeunit.md) | [administrativeUnit](administrativeunit.md)      | この**educationSchool**に対応する**administrativeUnit**を取得します。                |
| [Update](../api/educationschool-update.md)                                 | [educationSchool](educationschool.md)            | **educationSchool** オブジェクトを更新します。                                                       |
| [Delete](../api/educationschool-delete.md)                                 | None                                             | **educationSchool** オブジェクトを削除します。                                                       |
| [差分](../api/educationschool-delta.md)                                   | [educationSchool](educationschool.md) コレクション | **EducationSchools**の増分の変更を取得する                                            |

## <a name="properties"></a>プロパティ

| プロパティ            | 型                                  | 説明                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| id                  | 文字列                                | この学校の GUID。                               |
| address             | [physicalAddress](physicaladdress.md) | 学校の住所。                             |
| createdBy           | [identitySet](identityset.md)         | 学校を作成したエンティティ。                     |
| description         | String                                | 学校の説明。                         |
| displayName         | String                                | 学校の表示名。                        |
| externalId          | String                                | 同期システム内の学校の ID。                    |
| externalPrincipalId | String                                | 同期システム内のプリンシパルの ID。                 |
| externalSource      | string                                | 読み取り専用。 使用可能な値: `sis` または `manual`。 |
| fax                 | String                                | 学校の FAX 番号。                              |
| highestGrade        | String                                | 授業を受けている最高学年。                              |
| lowestGrade         | String                                | 授業を受けている最低学年。                               |
| phone               | String                                | 学校の電話番号。                            |
| principalEmail      | String                                | プリンシパルの電子メール アドレス。                    |
| principalName       | String                                | プリンシパルの名前。                             |
| schoolNumber        | String                                | 学校番号。                                     |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                                           | 説明                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| classes      | [educationClass](educationclass.md) コレクション | 学校で授業しているクラス。 Null 許容型。 |
| users        | [educationUser](educationuser.md) コレクション   | 学校のユーザー。 Null 許容型。          |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
"blockType": "resource",
"keyProperty": "id",
"optionalProperties": [

],
"@odata.type": "microsoft.graph.educationSchool"
}-->


```json
{
  "address": { "@odata.type": "microsoft.graph.physicalAddress" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalPrincipalId": "String",
  "externalSource": "string",
  "fax": "String",
  "highestGrade": "String",
  "id": "String (identifier)",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationSchool has documented navigation properties, but we thought it was a complex type!" 
  ]  
}-->
