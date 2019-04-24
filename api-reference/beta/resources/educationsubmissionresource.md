---
title: educationSubmissionResource リソースの種類
description: '提出物で使用するためにリソースをラップするラッパー。 ラッパーは、割り当てからコピーされた場合、割り当てリソースへのポインターを追加します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef231de49d3871ec877c279b4e77585343e1a85e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507078"
---
# <a name="educationsubmissionresource-resource-type"></a>educationSubmissionResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提出物で使用するためにリソースをラップするラッパー。 ラッパーは、割り当てからコピーされた場合、割り当てリソースへのポインターを追加します。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[educationSubmissionResource を取得する](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |**educationSubmissionResource**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[削除する](../api/educationsubmissionresource-delete.md) | なし |**educationSubmissionResource**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|割り当て resourceurl|String|このリソースがコピーされた割り当てへのポインター。 この値が null の場合、学生はリソースをアップロードしました。|
|id|String| 読み取り専用です。|
|リソース|[educationResource](educationresource.md)|Resource オブジェクト。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
