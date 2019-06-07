---
title: educationUser リソースの種類
description: システム内のユーザーです。 これは教育機関に固有の、Microsoft Graph が教育機関に固有でない `/users` エンドポイントから返すものと同じ `id` を持つユーザーのバリアント型です。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 616c11bca1711dead0007d153b77bcf377490a7a
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750109"
---
# <a name="educationuser-resource-type"></a>educationUser リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

システム内のユーザーです。 これは教育機関に固有の、Microsoft Graph が教育機関に固有でない `/users` エンドポイントから返すものと同じ `id` を持つユーザーのバリアント型です。
このオブジェクトは、コア [user] オブジェクトから対象のサブセットのプロパティを提供し、`primaryRole`、学生、教師データなど教育機関に固有のプロパティのセットを追加します。

## <a name="methods"></a>メソッド

| メソッド                                               | 戻り値の型                                  | 説明                                                                   |
| :--------------------------------------------------- | :------------------------------------------- | :---------------------------------------------------------------------------- |
| [Get educationUser](../api/educationuser-get.md)     | [educationUser]                              | **educationUser** オブジェクトのプロパティとリレーションシップを読み取ります。             |
| [List classes](../api/educationuser-list-classes.md) | [educationClass] コレクション                  | ユーザーがメンバーになっている **educationClass** オブジェクトのコレクションを取得します。    |
| [List schools](../api/educationuser-list-schools.md) | [educationSchool] コレクション                 | ユーザーがメンバーになっている **educationSchool** オブジェクトのコレクションを取得します。 |
| [Get user](../api/educationuser-get-user.md)         | [user]                                       | この **educationUser** に対応する単純なディレクトリ **user** を取得します。 |
| [Update](../api/educationuser-update.md)             | [educationUser]                              | **educationUser** オブジェクトを更新します。                                           |
| [Delete](../api/educationuser-delete.md)             | None                                         | **educationUser** オブジェクトを削除します。                                           |
| [差分](../api/educationuser-delta.md)               | [educationUser](educationuser.md) コレクション | **EducationUsers**の増分の変更を取得します。                               |

## <a name="properties"></a>プロパティ

| プロパティ          | 型                                                  | 説明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| :---------------- | :---------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                | 文字列                                                | ユーザーの一意の識別子。[directoryObject] から継承されます。キー。null 許容ではありません。読み取り専用です。                                                                                                                                                                                                                                                                                                                                                                                                                              |
| accountEnabled    | Boolean                                               | アカウントが有効な場合は **true**。それ以外の場合は **false**。 このプロパティは、ユーザーの作成時に必要です。 フィルター \$をサポートします。                                                                                                                                                                                                                                                                                                                                                                                                   |
| assignedLicenses  | [assignedLicense] collection                          | ユーザーに割り当てられているライセンス。null 許容ではありません。                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| assignedPlans     | [assignedPlan] collection                             | ユーザーに割り当てられているプラン。読み取り専用です。null 許容ではありません。                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| businessPhones    | String collection                                     | ユーザーの電話番号。 **メモ:** 文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。                                                                                                                                                                                                                                                                                                                                                                                                |
| createdBy         | [identitySet]                                         | ユーザーを作成したエンティティ。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| department        | String                                                | ユーザーが働いている部門の名前。 フィルター \$をサポートします。                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| displayName       | 文字列型 (String)                                                | アドレス帳に表示されるユーザーの名前。 これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 $filter および $orderby をサポートします。                                                                                                                                                                                                                                                           |
| externalSource    | `educationExternalSource`                             | このユーザーが作成された場所。 使用可能な値: `sis` または `manual`。                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| givenName         | String                                                | ユーザーの名。 フィルター \$をサポートします。                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| mail              | String                                                | ユーザーの SMTP アドレス (たとえば、"jeff@contoso.onmicrosoft.com")。 読み取り専用。 フィルター \$をサポートします。                                                                                                                                                                                                                                                                                                                                                                                                                        |
| mailNickname      | String                                                | ユーザーの電子メール エイリアス。 ユーザーの作成時に、このプロパティを指定する必要があります。 フィルター \$をサポートします。                                                                                                                                                                                                                                                                                                                                                                                                                          |
| mailingAddress    | [physicalAddress]                                     | ユーザーのメール アドレス。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| middleName        | String                                                | ユーザーのミドル ネーム。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mobilePhone       | String                                                | ユーザーの主な携帯電話の番号。                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| onPremisesInfo    | [educationOnPremisesInfo](educationonpremisesinfo.md) | AAD ユーザーを Active Directory に対応させるために使用される追加情報。                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| passwordPolicies  | String                                                | ユーザーのパスワード ポリシーを指定します。 この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。 "DisablePasswordExpiration" を指定することもできます。 2 つを一緒に指定できます。例: "DisablePasswordExpiration、DisableStrongPassword"。                                                                                                                                                                      |
| passwordProfile   | [passwordProfile]                                     | ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。                                                                                                                                                                                                                             |
| preferredLanguage | String                                                | ユーザーが設定する言語。 ISO 639-1 コードに従う必要があります。例: "en-US"。                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| primaryRole       | string                                                | ユーザーの既定のロール。 ユーザーのロールは、個々のクラスで異なる場合があります。 使用可能な値: `student`、`teacher`、`faculty`。 フィルター \$をサポートします。                                                                                                                                                                                                                                                                                                                                                                     |
| provisionedPlans  | [provisionedPlan]コレクション                          | ユーザーのために用意されたプラン。読み取り専用です。null 許容ではありません。                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| residenceAddress  | [physicalAddress]                                     | ユーザーが在住している場所のアドレス。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| student           | [educationStudent]                                    | プライマリ ロールが学生の場合、このブロックには学生固有のデータが含まれます。                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| surname           | String                                                | ユーザーの姓。 フィルター \$をサポートします。                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| teacher           | [educationTeacher]                                    | プライマリ ロールが教師の場合、このブロックには教師固有のデータが含まれます。                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| usageLocation     | String                                                | 2 文字の国コード (ISO 規格 3166) 国や地域におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。 たとえば、"US"、"JP"、"GB" などです。 null 許容ではありません。 フィルター \$をサポートします。                                                                                                                                                                                                                                                               |
| userPrincipalName | String                                                | ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。 |
| userType          | String                                                | ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。 フィルター \$をサポートします。                                                                                                                                                                                                                                                                                                                                                                                                       |

>[!IMPORTANT]
>委任されたアクセス許可スコープを使用する場合、Graph は限られ`id`た`primaryRole`プロパティ`accountEnabled`セット`displayName`のみ`givenName`を`surname`返し`userPrincipalName`ます`userType`: `onPremisesInfo`、、、、、、、、。 アプリケーションで追加のプロパティが必要な場合は、アプリケーションのアクセス許可スコープを使用する必要があります。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ  | 型                         | 説明                                  |
| :------------ | :--------------------------- | :------------------------------------------- |
| assignments   | [educationAssignment]        | ユーザーの割り当てのリスト。 Null 許容型。  |
| classes       | [educationClass] コレクション  | ユーザーが属しているクラス。 Null 許容型。 |
| schools       | [educationSchool] コレクション | ユーザーが属している学校。 Null 許容型。 |
| taughtClasses | [educationClass] コレクション  | ユーザーが教師であるクラス。     |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "accountEnabled": true,
  "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
  "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
  "businessPhones": ["String"],
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "department": "String",
  "displayName": "String",
  "externalSource": "string",
  "givenName": "String",
  "id": "String (identifier)",
  "mail": "String",
  "mailNickname": "String",
  "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
  "middleName": "String",
  "mobilePhone": "String",
  "officeLocation": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  },
  "passwordPolicies": "String",
  "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
  "preferredLanguage": "String",
  "primaryRole": "string",
  "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
  "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
  "student": { "@odata.type": "microsoft.graph.educationStudent" },
  "surname": "String",
  "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationUser has documented navigation properties, but we thought it was a complex type!" 
  ]

}-->

[educationuser]: educationuser.md
[educationclass]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: educationassignment.md
[educationteacher]: educationteacher.md
[educationstudent]: educationstudent.md
[relatedcontact]: relatedcontact.md
[physicaladdress]: physicaladdress.md
[provisionedplan]: provisionedplan.md
[passwordprofile]: passwordprofile.md
[identityset]: identityset.md
[assignedplan]: assignedplan.md
[assignedlicense]: assignedlicense.md
[ユーザー]: user.md
[directoryobject]: directoryobject.md
