---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 97265c1d6c36e425b312e088e6078341a2cff5b8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993530"
---
# <a name="update-user"></a>ユーザーを更新する

ユーザー オブジェクトのプロパティを更新します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | User.ReadWrite、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | User.ReadWrite    |
|アプリケーション | User.ReadWrite.All、Directory.ReadWrite.All |

>[!NOTE]
> - **passwordProfile** プロパティを更新するときは、次のアクセス許可が必要です。Directory.AccessAsUser.All。
> - 他のユーザーの**businessPhones**、**mobilePhone**、または**otherMails** のプロパティの更新を許可されているのは、管理者以外のユーザーまたは次のロールのいずれかを割り当てられたユーザーのみになります。ディレクトリ閲覧者、ゲスト招待元、メッセージ センター閲覧者およびレポート閲覧者。 詳細については、「[Azure AD で使用できるロール](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)」のヘルプデスク (パスワード) 管理者を参照してください。  User.ReadWrite.All または Directory.ReadWrite.All の委任またはアプリケーションのアクセス許可のいずれかが与えられているアプリの場合、これに該当します。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値|
|:-----------|:------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|aboutMe|String|ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。|
|accountEnabled|ブール値| アカウントが有効な場合は **true**。そうでない場合は **false**。 このプロパティは、ユーザーの作成時に必要です。    |
|birthday|DateTimeOffset|ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|businessPhones| String collection | ユーザーの電話番号。注:文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。|
|city|String|ユーザーがいる都市。|
|country|String|ユーザーがいる国/地域。たとえば、「US (米国)」や「UK (英国)」です。|
|department|String|ユーザーが働いている部門の名前。|
|displayName|String|アドレス帳に表示されるユーザーの名前。これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせです。このプロパティは、ユーザーの作成時に必須になります。更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|givenName|String|ユーザーの名。|
|hireDate|DateTimeOffset|ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|interests|String collection|ユーザーが自分の関心事を記述する一覧。|
|jobTitle|String|ユーザーの役職。|
|mailNickname|String|ユーザーの電子メール エイリアス。 ユーザーの作成時に、このプロパティを指定する必要があります。|
|mobilePhone|String|ユーザーの主な携帯電話の番号。|
|mySite|String|ユーザーの個人用サイトの URL。|
|officeLocation|String|ユーザーの勤務先の場所。|
|onPremisesImmutableId|String|このプロパティは、オンプレミスの Active Directory ユーザー アカウントを Azure AD ユーザー オブジェクトに関連付けるために使用します。 Graph で新しいユーザー アカウントを作成するとき、ユーザーの **userPrincipalName** (UPN) プロパティにフェデレーション ドメインを使用する場合は、このプロパティを指定する必要があります。 **重要:** **$** と **_** の文字は、このプロパティを指定するときには使用できません。                            |
|otherMails|String |ユーザーの追加のメール アドレスの一覧 (例: `["bob@contoso.com", "Robert@fabrikam.com"]`)。|
|passwordPolicies|String|ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。|
|pastProjects|String collection|ユーザーが過去のプロジェクトを列挙する一覧。|
|postalCode|String|ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。|
|preferredLanguage|String|ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。|
|responsibilities|String collection|ユーザーが自分の責任の範囲を列挙する一覧。|
|schools|String collection|ユーザーが在籍した学校を列挙する一覧。|
|skills|String collection|ユーザーが自分のスキルを列挙する一覧。|
|state|String|ユーザーの住所の都道府県。|
|streetAddress|String|ユーザーの勤務先の番地。|
|surname|String|ユーザーの姓。|
|usageLocation|String|2 文字の国コード (ISO 規格 3166) 国におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。  たとえば、"US"、"JP"、"GB" などです。 null 許容ではありません。|
|userPrincipalName|String|ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](../resources/organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。
|userType|String|ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。          |

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
##### <a name="response"></a>応答
以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
