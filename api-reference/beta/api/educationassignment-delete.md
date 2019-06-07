---
title: EducationAssignment の削除
description: 既存の割り当てを削除します。 割り当てを削除できるのは、クラス内の教師だけです。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 10a66116b9fb3443cce72641fd8ffb7f63d6fee0
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750039"
---
# <a name="delete-educationassignment"></a>EducationAssignment の削除

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

既存の割り当てを削除します。 割り当てを削除できるのは、クラス内の教師だけです。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)             |
| :------------------------------------- | :------------------------------------------------------ |
| 委任 (職場または学校のアカウント)     | EduAssignments の読み取り/書き込みの EduAssignments |
| 委任 (個人用 Microsoft アカウント) | サポートされません。                                          |
| アプリケーション                            | サポートされません。                                          |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                     |
| :------------ | :------------------------ |
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a>応答
応答の例を次に示します。 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

#### <a name="sdk-sample-code"></a>SDK サンプル コード

# <a name="ctabcs"></a>[C#](#tab/cs)

[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)

[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
