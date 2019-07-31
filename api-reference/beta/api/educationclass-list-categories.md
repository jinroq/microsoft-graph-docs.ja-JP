---
title: リスト educationCategories
description: Category オブジェクトのリストを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6757f64942ee87d4e13b577964645f9a35839477
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955426"
---
# <a name="list-educationcategories"></a>リスト educationCategories

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[EducationCategory](../resources/educationcategory.md)オブジェクトのリストを取得します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| 委任 (職場または学校のアカウント)     | EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本 |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                                                                                         |
| アプリケーション                            | サポートされていません。                                                                                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                     |
| :------------ | :------------------------ |
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationCategory](../resources/educationcategory.md)オブジェクトのコレクションを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories
```

##### <a name="response"></a>応答

応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }, {
        "displayName": "Homework",
        "id": "3943e9ea-c69b-4dc9-9674-5f24168cee35"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
