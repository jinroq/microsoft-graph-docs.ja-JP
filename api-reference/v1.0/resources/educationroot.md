---
title: educationRoot リソースの種類
description: '`/education` 名前空間は、教育機関に固有の機能を公開します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 84b7312515174c19837a5cda3fa3ffb466f65c23
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458755"
---
# <a name="educationroot-resource-type"></a>educationRoot リソースの種類

`/education` 名前空間は、教育機関に固有の機能を公開します。 `/education` 名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。 教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create educationClass](../api/educationroot-post-classes.md) |[educationClass](educationclass.md)| クラス コレクションに投稿して、新しい **educationClass** を作成します。|
|[List classes](../api/educationroot-list-classes.md) |[educationClass](educationclass.md) コレクション| **educationClass** オブジェクト コレクションを取得します。|
|[Create educationSchool](../api/educationroot-post-schools.md) |[educationSchool](educationschool.md)| 学校コレクションに投稿して、新しい **educationSchool** を作成します。|
|[List schools](../api/educationroot-list-schools.md) |[educationSchool](educationschool.md) コレクション| **educationSchool** オブジェクト コレクションを取得します。|
|[Create educationUser](../api/educationroot-post-users.md) |[educationUser](educationuser.md)| ユーザー コレクションに投稿して、新しい **educationUser** を作成します。|
|[List users](../api/educationroot-list-users.md) |[educationUser](educationuser.md) コレクション| **educationUser** オブジェクト コレクションを取得します。|

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) コレクション| 読み取り専用です。 Null 許容型。|
|me|[educationUser](educationuser.md)| 読み取り専用です。 Null 許容型。|
|schools|[educationSchool](educationschool.md) コレクション| 読み取り専用。Null 許容型。|
|users|[educationUser](educationuser.md) コレクション| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
