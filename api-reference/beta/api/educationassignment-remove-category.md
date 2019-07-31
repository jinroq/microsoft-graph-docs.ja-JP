---
title: EducationCategory の削除
description: 既存の educationCategory をこの educationAssignment から削除します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: deb55b14c40acb25b366eec140cbc433e9ee203d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955666"
---
# <a name="remove-educationcategory"></a>EducationCategory の削除

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[EducationAssignment](../resources/educationassignment.md)から[educationCategory](../resources/educationcategory.md)を削除します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  EduAssignments の読み取り/書き込みの EduAssignments  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | サポートされていません。  | 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。


## <a name="response"></a>応答
成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a>応答
応答の例を次に示します。 

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しではすべてのプロパティが返されます。


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
