---
title: 連絡先を更新する
description: 連絡先オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 95b19ff61cf39b9ad36c220ff7b4c4f5dd8cffce
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261307"
---
# <a name="update-contact"></a>連絡先を更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

連絡先オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Contacts.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Contacts.ReadWrite    |
|アプリケーション | Contacts.ReadWrite |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
ユーザーの既定の[Contactfolder](../resources/contactfolder.md)からの[連絡先](../resources/contact.md)。
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
[contactFolder](../resources/contact.md) の子フォルダー内に含まれる [連絡先](../resources/mailfolder.md)。  次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json. Required.  |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assistantName|String|連絡先のアシスタントの名前。|
|birthday|DateTimeOffset|連絡先の誕生日です。|
|categories|String|連絡先に関連付けられたカテゴリ。|
|children|String||
|companyName|String|連絡先の会社の名前。|
|department|String|連絡先の部署。|
|displayName|文字列|連絡先の表示名。 後で他のプロパティを更新すると、指定した displayName 値が自動的に生成された値に上書きされますので、ご注意ください。 既存の値を保持するには、[更新] 操作で必ずその値を displayName として含めてください。|
|emailAddresses|[typedEmailAddress](../resources/typedemailaddress.md)コレクション|連絡先のメール アドレス。|
|fileAs|String|連絡先がファイルされる名前。|
|gender |String |連絡先の性別。 |
|generation|String|連絡先の世代。|
|givenName|String|連絡先の名。|
|imAddresses|String|連絡先のインスタント メッセージング (IM) アドレス。|
|initials|String|連絡先のイニシャル。|
|jobTitle|String|連絡先の役職。|
|manager|String|連絡先の上司の名前。
|middleName|String|連絡先のミドル ネーム。|
|nickName|String|連絡先のニックネーム。|
|officeLocation|String|連絡先のオフィスの所在地。|
|parentFolderId|String|連絡先の親フォルダーの ID。|
|personalNotes|String|連絡先に関するユーザーのメモ。|
|phones |[phone](../resources/phone.md) コレクション |自宅電話、携帯電話、勤務先電話など、連絡先に関連付けられた電話番号。 |
|postalAddresses |[physicalAddress](../resources/physicaladdress.md)コレクション |自宅住所や勤務先住所など、連絡先に関連付けられた住所。 |
|profession|String|連絡先の専門的職業。|
|spouseName|String|連絡先の配偶者/パートナーの名前。|
|姓|文字列|連絡先の姓。|
|title|String|連絡先の肩書。|
|websites |[website](../resources/website.md) コレクション|連絡先に関連付けられた Web サイト。 |
|weddingAnniversary 日 |日付 |連絡先の結婚記念日。 |
|yomiCompanyName|String|連絡先の会社名の読み仮名。このプロパティは省略可能です。|
|yomiGivenName|文字列|連絡先の名 (ファースト ネーム) の読み仮名。このプロパティは省略可能です。|
|yomiSurname|String|連絡先の姓 (ラスト ネーム) の読み仮名。このプロパティは省略可能です。|

**Contact**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、操作を使用して、既存の**連絡先**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除することができます。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[連絡先](../resources/contact.md)オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の使用例は、指定された連絡先の個人用電子メールアドレスを更新します。
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_contact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_contact-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_contact-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
