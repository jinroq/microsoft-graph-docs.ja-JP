---
title: educationSubmission リソースの種類
description: 提出書類は、割り当てによって所有されます。 提出書類は、リソースを表しますが、個人 (またはグループ) および有効にするに割り当て、グレードとフィードバックが返されます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: aeeb1355da2ffcb0ebf561af2ecd15ac93221e26
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521426"
---
# <a name="educationsubmission-resource-type"></a>educationSubmission リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提出書類は、割り当てによって所有されます。 提出書類は、リソースを表しますが、個人 (またはグループ) および有効にするに割り当て、グレードとフィードバックが返されます。
割り当てを発行する際の提出書類が自動的に作成します。 提出書類は、2 つのリソースのリストを所有しています。 リソースでは、送信済みのリソースがアクティブになっている受講者がリソースを表すときに、領域を使用するユーザ/グループを表します。  

>**注:** 状態は読み取り専用およびオブジェクトがアクションを使用してワークフローを移動します。 

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[EducationSubmission を取得します。](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |**EducationSubmission**オブジェクトのプロパティと関係を参照してください。|
|[ボックスの一覧のリソース](../api/educationsubmission-list-resources.md) |[educationSubmissionResource](educationsubmissionresource.md)コレクション| **EducationSubmissionResource**オブジェクトのコレクションを取得します。|
|[リスト submittedResources](../api/educationsubmission-list-submittedresources.md) |[educationSubmissionResource](educationsubmissionresource.md)コレクション| **EducationSubmissionResource**オブジェクトのコレクションを取得します。|
|[Update](../api/educationsubmission-update.md) | [educationSubmission](educationsubmission.md) |**EducationSubmission**オブジェクトを更新します。 |
|[Return](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|教師は、生徒に成績とフィードバックを表示できることを示す戻り値を使用します。|
|[Submit](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|受講者にするには、割り当ての使用を送信します。 これは、グレーディングの**submittedResources**フォルダーにリソースをコピーし、ステータスを更新します。|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|受講者は、作業から提出された提出書類の状態に移動するのには、unsubmit を使用します。 これは、グレーディングの**workingResources**フォルダーにリソースをコピーし、ステータスを更新します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|feedback|[educationFeedback](educationfeedback.md)|受講者に、先生のノートを保存する [フィードバック] プロパティを保持します。|
|grade|[educationAssignmentGrade](educationassignmentgrade.md)|教師は、この送信に割り当てられますグレード情報を保持するには。|
|id|String| 読み取り専用。|
|Recipient|[educationSubmissionRecipient](educationsubmissionrecipient.md)|この提出書類に割り当てられました。|
|releasedBy|[identitySet](identityset.md)|リリースには、この送信のステータスを移動したユーザーです。|
|releasedDateTime|DateTimeOffset|提出書類がリリースされた時点での瞬間。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|返す|[identitySet](identityset.md)|返されるには、この送信のステータスを移動したユーザーです。|
|returnedDateTime|DateTimeOffset|提出書類が返された瞬間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|resourcesFolderUrl|String|この送信のためのリソースのすべてのファイル、フォルダーを格納する必要があります。|
|status|string| 読み取り専用。 使用可能な値: `working`、`submitted`、`released`、`returned`。|
|submittedBy|[identitySet](identityset.md)|送信済みの状態に、リソースを移動したユーザーです。|
|submittedDateTime|DateTimeOffset|提出書類を提出済みの状態に移動したときの時点です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|unsubmittedBy|[identitySet](identityset.md)|リソースを移動したユーザーからは、作業の状態に送信します。|
|unsubmittedDateTime|DateTimeOffset|移動するとき、提出書類がから送信、正常な状態に瞬間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|resources|[educationSubmissionResource](educationsubmissionresource.md)コレクション| Null 許容型。|
|submittedResources|[educationSubmissionResource](educationsubmissionresource.md)コレクション| 読み取り専用です。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "grade": {"@odata.type": "microsoft.graph.educationAssignmentGrade"},
  "id": "String (identifier)",
  "recipient": {"@odata.type": "microsoft.graph.educationSubmissionRecipient"},
  "returnedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "returnedDateTime": "String (timestamp)",
  "resourcesFolderUrl": "String",
  "status": "string",
  "submittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "submittedDateTime": "String (timestamp)",
  "unsubmittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "unsubmittedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
