---
title: 'educationSchool: delta'
description: 学校コレクション全体の完全な読み取りを行わずに、新しく作成または更新された教育機関を取得します。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ef31d8cfa9f7b3680c4371e87eb86a46051f75bf
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764766"
---
# <a name="educationschool-delta"></a>educationSchool: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校コレクション全体の完全な読み取りを行わずに、新しく作成または更新された教育機関を取得します。 詳細については、「 [Use delta query](/graph/delta-query-overview) 」を参照してください。

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
POST /education/schools/{id}/delta
POST /education/me/schools/{id}/delta
POST /education/users/{id}/schools/{id}/delta

```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
| :------------ | :------------ |
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSchool](../resources/educationschool.md) collection オブジェクトを返します。

## <a name="example"></a>例

次の例は、この API を呼び出す方法を示しています。

##### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/delta
```

##### <a name="response"></a>応答

応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "principalEmail": "principalEmail-value",
      "principalName": "principalName-value",
      "externalPrincipalId": "externalPrincipalId-value",
      "lowestGrade": "lowestGrade-value",
      "highestGrade": "highestGrade-value",
      "schoolNumber": "schoolNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
