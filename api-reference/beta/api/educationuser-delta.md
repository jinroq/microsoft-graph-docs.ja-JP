---
title: 'educationUser: delta'
description: ユーザーコレクション全体の完全な読み取りを実行せずに、新しく作成または更新されたユーザーを取得します。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c89c065d5e4bd8510d6821a3c7a13bd106ce9eb8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764764"
---
# <a name="educationuser-delta"></a>educationUser: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

コレクション全体の完全な読み取りを実行せずに、新しく作成または更新された[educationUser](../resources/educationuser.md)を取得します。 詳細については、「 [Use delta query](/graph/delta-query-overview) 」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)     |
| :------------------------------------- | :---------------------------------------------- |
| 委任 (職場または学校のアカウント)     | サポートされていません。                                  |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                                  |
| アプリケーション                            | Eduroster.readbasic または Eduroster.readbasic のいずれかを取得します。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
| :------------ | :------------ |
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationUser](../resources/educationuser.md) collection オブジェクトを返します。

## <a name="example"></a>例

次の例は、この API を呼び出す方法を示しています。

##### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a>応答

応答の例を次に示します。

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1039

{
  "value": [
    {
      "primaryRole": "primaryRole-value",
      "middleName": "middleName-value",
      "externalSource": "externalSource-value",
      "residenceAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "mailingAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "student": {
        "graduationYear": "graduationYear-value",
        "grade": "grade-value",
        "birthDate": "datetime-value",
        "gender": "gender-value",
        "studentNumber": "studentNumber-value",
        "externalId": "externalId-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
