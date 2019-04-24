---
title: educationUser リソースの種類
description: システム内のユーザーです。 これは教育機関に固有の、Microsoft Graph が教育機関に固有でない `/users` エンドポイントから返すものと同じ `id` を持つユーザーのバリアント型です。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4a1caaa7d81540f6a90052b13f04d7d3e5bf77da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463566"
---
# <a name="educationuser-resource-type"></a>educationUser リソースの種類

システム内のユーザーです。 これは教育機関に固有の、Microsoft Graph が教育機関に固有でない `/users` エンドポイントから返すものと同じ `id` を持つユーザーのバリアント型です。
このオブジェクトは、コア [user](user.md) オブジェクトから対象のサブセットのプロパティを提供し、`primaryRole`、学生、教師データなど教育機関に固有のプロパティのセットを追加します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get educationUser](../api/educationuser-get.md) | [educationUser](educationuser.md) |**educationUser** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[List classes](../api/educationuser-list-classes.md) |[educationClass](educationclass.md) コレクション| ユーザーがメンバーになっている **educationClass** オブジェクトのコレクションを取得します。|
|[List schools](../api/educationuser-list-schools.md) |[educationSchool](educationschool.md) コレクション| ユーザーがメンバーになっている **educationSchool** オブジェクトのコレクションを取得します。|
|[Get user](../api/educationuser-get-user.md) |[user](user.md)| この **educationUser** に対応する単純なディレクトリ **user** を取得します。|
|[Update](../api/educationuser-update.md) | [educationUser](educationuser.md)   |**educationUser** オブジェクトを更新します。 |
|[削除する](../api/educationuser-delete.md) | なし |**educationUser** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| アカウントが有効な場合は **true**。それ以外の場合は **false**。 このプロパティは、ユーザーの作成時に必要です。 $filter をサポートします。    |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|ユーザーに割り当てられているライセンス。null 許容ではありません。            |
|assignedPlans|[assignedPlan](assignedplan.md) collection|ユーザーに割り当てられているプラン。読み取り専用です。null 許容ではありません。 |
|businessPhones|String collection|ユーザーの電話番号。 **メモ:** 文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。|
|createdBy|[identitySet](identityset.md)| ユーザーを作成したエンティティ。 |
|department|String|ユーザーが働いている部門の名前。$filter をサポートします。|
|displayName|文字列型 (String)|アドレス帳に表示されるユーザーの名前。 これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 $filter および $orderby をサポートします。|
|externalSource|`educationExternalSource`| このユーザーが作成された場所。 使用可能な値: `sis`、`manual`、`unkownFutureValue`。|
|givenName|String|ユーザーの名。$filter をサポートします。|
|id|String|ユーザーの一意の識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。|
|mail|String|ユーザーの SMTP アドレス (たとえば、"jeff@contoso.onmicrosoft.com")。 読み取り専用。 $filter をサポートします。|
|mailingAddress|[physicalAddress](physicaladdress.md)| ユーザーのメール アドレス。|
|mailNickname|String|ユーザーの電子メール エイリアス。ユーザーの作成時に、このプロパティを指定する必要があります。$filter をサポートします。|
|middleName| String | ユーザーのミドル ネーム。|
|mobilePhone|String|ユーザーの主な携帯電話の番号。|
|passwordPolicies|String|ユーザーのパスワード ポリシーを指定します。 この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。 "DisablePasswordExpiration" を指定することもできます。 2 つを一緒に指定できます。例: "DisablePasswordExpiration、DisableStrongPassword"。|
|passwordProfile|[PasswordProfile](passwordprofile.md)|ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。|
|preferredLanguage|String|ユーザーが設定する言語。 ISO 639-1 コードに従う必要があります。例: "en-US"。|
|primaryRole|educationUserRole| ユーザーの既定のロール。 ユーザーのロールは、個々のクラスで異なる場合があります。 使用可能な値: `student`、`teacher`、`unknownFutureValue`。 $filter をサポートします。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) collection|ユーザーのために用意されたプラン。読み取り専用です。null 許容ではありません。 |
|その他の連絡先|その他の[連絡先](relatedcontact.md)コレクション|ユーザーに関連する連絡先のセット。  このオプションのプロパティは $select 句で指定する必要があり、個々のユーザーに対してのみ取得できます。|
|residenceAddress|[physicalAddress](physicaladdress.md)| ユーザーが在住している場所のアドレス。|
|student|[educationStudent](educationstudent.md)| プライマリ ロールが学生の場合、このブロックには学生固有のデータが含まれます。|
|surname|String|ユーザーの姓。$filter をサポートします。|
|teacher|[educationTeacher](educationteacher.md)| プライマリ ロールが教師の場合、このブロックには教師固有のデータが含まれます。|
|usageLocation|String|2 文字の国コード (ISO 規格 3166) 国や地域におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。 たとえば、"US"、"JP"、"GB" などです。 null 許容ではありません。 $filter をサポートします。|
|userPrincipalName|文字列|ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。
|userType|String|ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。$filter をサポートします。          |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) コレクション| ユーザーが属しているクラス。 Null 許容型。|
|schools|[educationSchool](educationschool.md) コレクション| ユーザーが属している学校。 Null 許容型。|
|assignments| [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta)| ユーザーの割り当てのリスト。 Null 許容型。|
|user|[ユーザー](user.md)| このユーザーに対応するディレクトリユーザー。|

>**メモ:**  **educationassignment** リソースは /beta ベータ版のリソースです。 このリソースを使用する場合は、[変更ログ](/graph/changelog)を定期的に確認してください。 Microsoft Graph API リソースが /v1.0 エンドポイントにリリースされると、リリースは変更ログに記録されます。 アプリが **educationassignment** リソースを使用する場合は、次のコード ブロックに示すように、基本要求 URL を宣言する必要があります。  
```JavaScript
var v1BaseUrl = “https://graph.microsoft.com/v1.0/education”;
var betaBaseUrl = “https://graph.microsoft.com/beta/education”;  // for administrativeUnit and educationOrganization
```


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "accountEnabled": true,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["555-555-6568"],
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "preferredLanguage": "string",
  "primaryRole": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"},
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: microsoft.graph.educationUser/assignments:
      Referenced type microsoft.graph.educationAssignment is not defined in the doc set! Potential suggestion: UNKNOWN",
    "Warning: /api-reference/v1.0/resources/educationuser.md/microsoft.graph.educationUser:
      Property 'relatedContacts' found in markdown table but not in resource definition."
  ],
  "tocPath": ""
}-->
