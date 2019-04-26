---
title: educationCategories の追加
description: 既存の educationCategory をこの educationAssignment に追加する
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: afb89d40dd0f074da9ef1f6c7b0aeb1ff952c43f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325217"
---
# <a name="add-educationcategories"></a>educationCategories の追加

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この[educationAssignment](../resources/educationassignment.md)に、1つ以上の既存の[educationCategory](../resources/educationcategory.md)オブジェクトを追加します。

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
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、この割り当てに追加する既存の[educationCategory](../resources/educationcategory.md)オブジェクトの odata.id を指定します。


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
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/11021/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
要求本文で、この割り当てに追加する既存の[educationCategory](../resources/educationcategory.md)オブジェクトの odata.id を指定します。
##### <a name="response"></a>応答
応答の例を次に示します。 

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 すべてのプロパティは実際の呼び出しから返されます。


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
  "description": "Add educationCategory to educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
