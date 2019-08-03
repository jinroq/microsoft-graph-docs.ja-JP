---
title: educationAssignment リソースの種類
description: '**EducationAssignment**リソースは、クラス内の学生またはチームメンバーに割り当てられた作業の1つまたは複数の作業単位を調査の一環として表します。 割り当てを作成できるのは、教師またはチームの所有者のみです。 割り当てには、教師が学生の作業を希望する配布資料とタスクが含まれています。 各受講者の割り当てには、教師が有効にすることを求められた仕事がすべて含まれている送信が関連付けられています。 教師は、生徒が行った提出物にスコアとフィードバックを追加することができます。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1f343edec96af2e51d1bb643abb0652425c54624
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173049"
---
# <a name="educationassignment-resource-type"></a>educationAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**EducationAssignment**リソースは、クラス内の学生またはチームメンバーに割り当てられた作業の1つまたは複数の作業単位を調査の一環として表します。 割り当てを作成できるのは、教師またはチームの所有者のみです。 割り当てには、教師が学生の作業を希望する配布資料とタスクが含まれています。 各受講者の割り当てには、教師が有効にすることを求められた仕事がすべて含まれている[送信](educationsubmissionresource.md)が関連付けられています。 教師は、生徒が行った提出物にスコアとフィードバックを追加することができます。

割り当てが作成されると、その割り当ては下書き状態になります。 学生は、割り当てを表示できません。送信は作成されません。 "[発行](../api/educationassignment-publish.md)" アクションを使用して、割り当ての状態を変更できます。 PATCH 要求を使用して割り当ての状態を変更することはできません。

割り当て Api は、クラスの名前空間で公開されます。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リソースを一覧表示する](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md)コレクション| **EducationAssignmentResource**オブジェクトのコレクションを取得します。|
|[送信の一覧表示](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md)コレクション| **EducationSubmission**オブジェクトのコレクションを取得します。|
|[カテゴリの一覧表示](../api/educationassignment-list-categories.md) |[educationCategory](educationcategory.md)コレクション| **EducationCategory**オブジェクトのコレクションを取得します。|
|[割り当てリソースを作成する](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Resources コレクションへの投稿によって新しい**educationAssignmentResource**を作成します。|
|[割り当てを取得する](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |**EducationAssignment**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |**EducationAssignment**オブジェクトを更新します。 |
|[Delete](../api/educationassignment-delete.md) | None |**EducationAssignment**オブジェクトを削除します。 |
|[カテゴリを追加する](../api/educationassignment-add-categories.md) |[educationCategory](educationcategory.md) | クラスに属する**educationCategory**をこの割り当てに割り当てます。|
|[カテゴリを削除する](../api/educationassignment-remove-category.md) |None| クラスに属する**educationCategory**をこの割り当てから削除します。|
|[割り当てを適用する (ic)](../api/educationassignment-put-rubric.md)|None|既存の**educationRubric**をこの割り当てに添付します。|
|[の削除](../api/educationassignment-delete-rubric.md)|None|この割り当てから**educationRubric**を切断します。|
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|**EducationAssignment**オブジェクトの状態を下書きから発行済みに変更します。|
|[リソース フォルダーの URL を取得する](../api/educationassignment-getresourcesfolderurl.md)| string| 割り当てリソースの一部として、ファイルベースのリソースが配置される OneDrive フォルダーです。 ファイルをリソースとして追加するには、このフォルダーに配置する必要があります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。|
|allowLateSubmissions|Boolean| 学生が期日を過ぎて送信できるかどうかを指定します。 このプロパティが作成時に指定されていない場合、既定値は true になります。 |
|allowStudentsToAddResourcesToSubmission|Boolean| 学生が自分のリソースを提出することができるかどうか、または教師が追加したリソースのみを変更できるかどうかを識別します。 |
|割り当ての Datetime|DateTimeOffset|割り当てがアクティブになる日付を指定します。  今後、この日まで学生に割り当てが表示されることはありません。  **Timestamp**型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|への割り当て|[educationAssignmentRecipient](educationassignmentrecipient.md)| 割り当てが発行されると、どのユーザーまたはクラス全体が送信オブジェクトを受け取るかを指定します。 |
|assignedDateTime|DateTimeOffset|割り当てが学生に公開され、課題が生徒のタイムラインに表示されます。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|classId|String| この割り当てが属するクラス。 |
|createdBy|[identitySet](identityset.md)| 割り当てを作成したユーザー。 |
|createdDateTime|DateTimeOffset|割り当てが作成された瞬間。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|displayName|文字列|割り当ての名前を指定します。|
|dueDateTime|DateTimeOffset|学生の割り当てが期限になる日付。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|変化|[educationAssignmentGradeType](educationassignmentgradetype.md)|割り当てが採点される方法。 |
|手順|[itemBody](itembody.md)| 割り当ての手順。  これに加えて、表示名と共に、受講者に実行する操作を指示します。 |
|lastModifiedBy|[identitySet](identityset.md)| 割り当てを最後に変更したユーザー。 |
|lastModifiedDateTime|DateTimeOffset|割り当てが最後に変更された瞬間。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|status|string| **割り当て**の状態。  この値を修正することはできません。  可能な値は、`draft`、`published`、`assigned` です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[educationAssignmentResource](educationassignmentresource.md)コレクション| この割り当てに関連付けられているオブジェクトを学習します。  このリストは教師のみが変更できます。 Null 許容型。|
|投稿|[educationSubmission](educationsubmission.md)コレクション| 発行された後に、各学生の仕事と成績を表す送信オブジェクトがあります。  読み取り専用です。 Null 許容型。|
|categories|[educationCategory](educationcategory.md)コレクション| 設定されている場合、ユーザーは特定の種類の割り当てを簡単に見つけることができます。  読み取り専用です。 Null 許容型。|
|rubric|[educationRubric](educationrubric.md)|設定すると、この割り当てに関連付けられている、適用されます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "String (timestamp)",
  "classId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "dueDateTime": "String (timestamp)",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "instructions": {"@odata.type": "microsoft.graph.itemBody"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
