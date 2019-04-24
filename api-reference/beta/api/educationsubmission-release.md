---
title: 'educationSubmission: release'
description: " を指定します。 このアクションは教師のみが実行できます。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fb8d9ce6646cb7055f2edb4cc56c7d9784d96915
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464498"
---
# <a name="educationsubmission-release"></a>educationSubmission: release

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この操作によって、この送信に関連付けられている成績とフィードバックが学生に提供されます。 これにより、送信の状態が "送信済み" から "リリース済み" に変更され、変更が行われたことが示されます。 このアクションは教師のみが実行できます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  EduAssignments の読み取り/書き込みの EduAssignments   |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | サポートされていません。 | 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
次の例は、この API を呼び出す方法を示しています。
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a>応答
応答の例を次に示します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-release.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
