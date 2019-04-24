---
title: educationassignment の更新
description: assignment オブジェクトを更新します。 この操作を行うことができるのは、クラス内の教師だけです。 PATCH 要求を使用して割り当ての状態を変更することはできないことに注意してください。 割り当ての状態を変更するには、発行アクションを使用します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb5762f86e1572f9a9d5876199c945154a25293b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458167"
---
# <a name="update-educationassignment"></a>educationassignment の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

assignment オブジェクトを更新します。 この操作を行うことができるのは、クラス内の教師だけです。 PATCH 要求を使用して割り当ての状態を変更することはできないことに注意してください。 割り当ての状態を変更するには、[発行](../api/educationassignment-publish.md)アクションを使用します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  EduAssignments の読み取り/書き込みの EduAssignments  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | サポートされていません。 | 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowLateSubmissions|Boolean| 期日後に提出を送信できるかどうか。|
|allowStudentsToAddResourcesToSubmission|Boolean| 学生が提出物にリソースを追加できるかどうか。 提出物のアイテムが割り当てリソースリストからのものだけであったかどうかを示しました。 |
|割り当ての datetime|DateTimeOffset| 割り当てが学生に公開される日付。 |
|への割り当て|educationAssignmentRecipient| 課題を受ける学生。|
|displayName|String| 割り当ての名前を指定します。 |
|dueDateTime|DateTimeOffset| 日付の割り当て期限です。 |
|変化|educationAssignmentGradeType| 割り当てが採点される方法。|
|手順|microsoft.outlookservices.itembody| 受講者に割り当てと共に提供される指示。 |

## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[educationAssignment](../resources/educationassignment.md)オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
}
```
##### <a name="response"></a>応答
応答の例を次に示します。 

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 すべてのプロパティは実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
