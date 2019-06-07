---
title: educationSchool に educationUser を追加する
description: 学校にユーザーを追加します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a50414de93cec213bc76d626a3a4d6873738e41e
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34749983"
---
# <a name="add-educationuser-to-an-educationschool"></a>educationSchool に educationUser を追加する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校にユーザーを追加します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | サポートされていません。                              |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                              |
| アプリケーション                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                     |
| :------------ | :------------------------ |
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type  | application/json          |

## <a name="request-body"></a>要求本文

要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->

```http
POST https://graph.microsoft.com/beta/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14008"
}
```

##### <a name="response"></a>応答

応答の例を次に示します。 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->

```http
HTTP/1.1 204 No Content
```

#### <a name="sdk-sample-code"></a>SDK サンプル コード

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)

[!INCLUDE [sample-code](../includes/create_educationuser_from_educationschool-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
