---
title: 'educationClass: delta'
description: クラスコレクション全体の完全な読み取りを実行しなくても、メンバーシップの変更など、新しく作成された、または更新されたクラスを取得します。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 03a026a479c9502e00b86e41936619613013b9af
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764763"
---
# <a name="educationclass-delta"></a>educationClass: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

クラスコレクション全体の完全な読み取りを実行しなくても、メンバーシップの変更など、新しく作成された、または更新されたクラスを取得します。 詳細については、「 [Use delta query](/graph/delta-query-overview) 」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| 委任 (職場または学校のアカウント)     | Eduroster.readbasic、Eduroster.readbasic、または Eduroster.readbasic の読み取り/書き込み              |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                                                           |
| アプリケーション                            | Eduroster.readbasic、Eduroster.readbasic、または Eduroster.readbasic のすべての値を取得します。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
| :------------ | :------------ |
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationClass](../resources/educationclass.md) collection オブジェクトを返します。

## <a name="example"></a>例

次の例は、この API を呼び出す方法を示しています。

##### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a>応答

応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "displayName": "displayName-value",
      "mailNickname": "mailNickname-value",
      "description": "description-value",
      "createdBy": {
        "application": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "device": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "user": {
          "displayName": "displayName-value",
          "id": "id-value"
        }
      },
      "classCode": "classCode-value",
      "externalName": "externalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
