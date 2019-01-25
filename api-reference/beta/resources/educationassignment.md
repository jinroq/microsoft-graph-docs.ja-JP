---
title: educationAssignment リソースの種類
description: '**EducationAssignment**リソースは、タスクや、研究の一部として、クラスの受講生受講者またはチームのメンバーに割り当てられた作業時間の単位を表します。 教師またはチームの所有者のみが、割り当てを作成できます。 配布資料と講師が、受講生受講者の作業をしようとしているタスクの割り当てが含まれています。 各受講生受講者の割り当てには、関連する送信の小学校は、オンする作業が含まれています。 教師では受講者に提出するスコアとフィードバックを追加できます。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 68bb881800e1c63acb588e39bb64e1d02e005cc3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508959"
---
# <a name="educationassignment-resource-type"></a>educationAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**EducationAssignment**リソースは、タスクや、研究の一部として、クラスの受講生受講者またはチームのメンバーに割り当てられた作業時間の単位を表します。 教師またはチームの所有者のみが、割り当てを作成できます。 配布資料と講師が、受講生受講者の作業をしようとしているタスクの割り当てが含まれています。 各受講生受講者の割り当てには、その小学校は、オンする作業が含まれている関連する[提出書類](educationsubmissionresource.md)があります。 教師では受講者に提出するスコアとフィードバックを追加できます。

割り当てを作成するときは、下書きの状態では。 受講者の割り当てが表示ことはできませんし、提出書類は作成されません。 [発行](../api/educationassignment-publish.md)操作を使用して、割り当ての状態を変更できます。 修正プログラムの要求は、割り当ての状態を変更するのには使用できません。

割り当て Api は、クラスの名前空間で公開されます。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[割り当てを取得します。](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |**EducationAssignment**オブジェクトのプロパティと関係を参照してください。|
|[割り当てリソースを作成します。](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| リソースのコレクションへの投稿には、新しい**educationAssignmentResource**を作成します。|
|[ボックスの一覧のリソース](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md)コレクション| **EducationAssignmentResource**オブジェクトのコレクションを取得します。|
|[ボックスの一覧の送信](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md)コレクション| **EducationSubmission**オブジェクトのコレクションを取得します。|
|[Update](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |**EducationAssignment**オブジェクトを更新します。 |
|[Delete](../api/educationassignment-delete.md) | なし |**EducationAssignment**オブジェクトを削除します。 |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|下書きを公開するからには、 **educationAssignment**オブジェクトの状態を変更します。|
|[リソース フォルダーの URL を取得します。](../api/educationassignment-getresourcesfolderurl.md)| string| OneDrive フォルダーには、割り当てリソースの一部とするファイル ベースのリソースを配置します。 リソースとして追加するには、このフォルダーにファイルを配置する必要があります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|文字列| 読み取り専用です。|
|allowLateSubmissions|ブール値| 受講者が期限より後に送信できるかどうかを識別します。 作成中にこのプロパティを指定しない場合の既定値は true です。 |
|allowStudentsToAddResourcesToSubmission|ブール値| 受講者が提出書類に独自のリソースを追加できるかどうか、またはかどうかのみ変更できる、先生によって追加のリソースを識別します。 |
|assignDateTime|DateTimeOffset|日付と割り当てをアクティブになります。  今後は場合、割り当ては表示されません、受講生受講者にこの日まで。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| ユーザー、または全体のクラスは、割り当てが発行される送信オブジェクトを受信する必要があります。 |
|assignedDateTime|DateTimeOffset|受講者を割り当て、割り当てが発行された時点を受講者のタイムライン上示しています。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|classId|String| この割り当てが属するクラス。 |
|createdBy|[identitySet](identityset.md)| 割り当てを作成したとします。 |
|createdDateTime|DateTimeOffset|割り当てが作成された時点。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|displayName|String|割り当ての名前です。|
|dueDateTime|DateTimeOffset|受講者の割り当てを期限の日付。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|グレーディング|[educationAssignmentGradeType](educationassignmentgradetype.md)|どの割り当てが焼き付けるされます。 |
|手順|[itemBody](itembody.md)| 割り当ての説明です。  この表示名と受講者を指示を行います。 |
|lastModifiedBy|[identitySet](identityset.md)| 最後の割り当てを変更したユーザーです。 |
|lastModifiedDateTime|DateTimeOffset|割り当てが最後に修正された瞬間。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|status|string| **割り当て**の状態です。  しないことができますこの値を修正します。  可能な値は、`draft`、`published`、`assigned` です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|resources|[educationAssignmentResource](educationassignmentresource.md)コレクション| この割り当てに関連付けられているオブジェクトを学習します。  教師だけでは、このリストを変更できます。 Null 許容型。|
|Submissions|[educationSubmission](educationsubmission.md)コレクション| 発行されるとグレードを表す各受講者の提出書類のオブジェクトがあります。  読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
