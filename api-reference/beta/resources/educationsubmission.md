---
title: educationSubmission リソースの種類
description: 提出物は、割り当てによって所有されます。 提出は、個人 (またはグループ) が割り当てに対して有効になるリソースと、返される成績/フィードバックを表します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 81c194c08ddc5ed8f5acc38ae84a5478bb7e0229
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972524"
---
# <a name="educationsubmission-resource-type"></a>educationSubmission リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提出物は、割り当てによって所有されます。 提出は、個人 (またはグループ) が割り当てに対して有効になるリソースと、返される成績/フィードバックを表します。
割り当てが発行されると、提出物は自動的に作成されます。 送信では、2つのリソースリストが所有されています。 リソースは、送信されたリソースが、学生が積極的に有効にしたリソースを表している間、ユーザー/グループの作業領域を表します。  

>**注:** 状態は読み取り専用で、オブジェクトはアクションによってワークフローを通じて移動されます。 

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[EducationSubmission を取得する](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |**EducationSubmission**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[リソースを一覧表示する](../api/educationsubmission-list-resources.md) |[educationSubmissionResource](educationsubmissionresource.md)コレクション| **EducationSubmissionResource**オブジェクトのコレクションを取得します。|
|[SubmittedResources を一覧表示する](../api/educationsubmission-list-submittedresources.md) |[educationSubmissionResource](educationsubmissionresource.md)コレクション| **EducationSubmissionResource**オブジェクトのコレクションを取得します。|
|[Update](../api/educationsubmission-update.md) | [educationSubmission](educationsubmission.md) |**EducationSubmission**オブジェクトを更新します。 |
|[Return](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|教師は、return を使用して、成績/フィードバックを学生に表示できることを示します。|
|[Submit](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|学生は、submit を使用して割り当てを有効にします。 これにより、リソースが [対象] の [ **Submittedresources** ] フォルダーにコピーされ、状態が更新されます。|
|[送信取り消し](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|学生は、未送信を使用して、提出物の状態を送信前から作業に移行します。 これにより、リソースが**workingResources**フォルダーにコピーされて、状況を更新して更新します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|feedback|[educationFeedback](educationfeedback.md)|教師のメモを生徒に返すフィードバックプロパティを保持します。|
|grade|[educationAssignmentGrade](educationassignmentgrade.md)|教師がこの送信に割り当てる成績情報を保持します。|
|id|String| 読み取り専用。|
|受信者|[educationSubmissionRecipient](educationsubmissionrecipient.md)|この提出物が割り当てられるユーザー。|
|releasedBy|[identitySet](identityset.md)|この提出の状態をリリース済みに移動したユーザー。|
|releasedDateTime|DateTimeOffset|提出物がいつリリースされたかを示します。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|returnedBy|[identitySet](identityset.md)|この提出の状態を取得したユーザー。|
|returnedDateTime|DateTimeOffset|送信が返された瞬間の時間。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|resourcesFolderUrl|String|この送信のすべてのファイルリソースを格納する必要があるフォルダーです。|
|status|string| 読み取り専用。 使用可能な値: `working`、`submitted`、`released`、`returned`。|
|submittedBy|[identitySet](identityset.md)|リソースを送信済み状態に移行したユーザー。|
|submittedDateTime|DateTimeOffset|提出された状態に提出された時点の状態。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|未提出者|[identitySet](identityset.md)|提出されたリソースを作業中の状態に移行したユーザー。|
|非 Submitteddatetime|DateTimeOffset|提出物が送信されてから作業中の状態に移行した時点の状態です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[educationSubmissionResource](educationsubmissionresource.md)コレクション| Null 許容型。|
|submittedResources|[educationSubmissionResource](educationsubmissionresource.md)コレクション| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
    "feedback":{"@odata.type":"microsoft.graph.educationFeedback"},
    "grade":{"@odata.type":"microsoft.graph.educationAssignmentGrade"},
    "id":"String (identifier)",
    "recipient":{"@odata.type":"microsoft.graph.educationSubmissionRecipient"},
    "returnedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "returnedDateTime":"String (timestamp)",
    "resourcesFolderUrl":"String",
    "status":"string",
    "submittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "submittedDateTime":"String (timestamp)",
    "unsubmittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "unsubmittedDateTime":"String (timestamp)",
    "releasedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "releasedDateTime":"String (timestamp)"
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
  "suppressions": []
}
-->
