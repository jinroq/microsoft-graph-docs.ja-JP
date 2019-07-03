---
title: educationUser プロパティを更新する
description: '**educationuser** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4ba79c00d95764be03b98eac86d521debd808b19
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441171"
---
# <a name="update-educationuser-properties"></a>educationUser プロパティを更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**educationuser** オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  サポートされていません。  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName| 文字列| ユーザーの表示名|
|givenName| String | 名 |
|middleName| String | ユーザーのミドル ネーム|
|surname| String | ユーザーの姓|
|mail| String| メール アドレス|
|mobilePhone| String | ユーザーの携帯電話番号 |
|externalSource|string| 可能な値は、`sis`、`manual`、`enum_sentinel` です。|
|externalSource|string| このユーザーが作成された場所。  可能な値は、`sis`、`manual`、`enum_sentinel` です。|
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)| ユーザーのメール アドレス。|
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)| ユーザーが在住している場所のアドレス。|
|primaryRole|string| ユーザーの既定のロール。  ユーザーのロールは、個々のクラスで異なる場合があります。 使用可能な値: `student`、`teacher`、`enum_sentinel`。|
|student|[educationStudent](../resources/educationstudent.md)| プライマリ ロールが学生の場合、このブロックには学生固有のデータが含まれます。|
|teacher|[educationTeacher](../resources/educationteacher.md)| プライマリ ロールが教師の場合、このブロックには教師固有のデータが含まれます。|


## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationUser](../resources/educationuser.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
