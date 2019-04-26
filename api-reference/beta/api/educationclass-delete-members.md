---
title: 学生を削除する
description: educationClass から educationUser を削除する
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ac5ee332c58a070d9f25dfb3bde78177fb323b02
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324949"
---
# <a name="remove-a-student"></a>学生を削除する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationClass](../resources/educationclass.md) から [educationUser](../resources/educationuser.md) を削除する

>**メモ:** 教師_および_学生は、クラス **members** コレクションに所属します。 この API を呼び出す前に、削除する **educationUser** が教師でないことを確認してください。  [educationclass_list_teachers](educationclass-list-teachers.md) を呼び出して教師のリストを取得し、削除対象のユーザーのユーザー ID が返された教師リストにないことを確認します。

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
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。


## <a name="response"></a>応答
成功した場合、このメソッドは `204 No Content` 応答コードと空の応答本文を返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a>応答
応答の例を次に示します。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
