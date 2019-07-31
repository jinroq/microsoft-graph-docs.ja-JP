---
title: educationSubmissionResource リソースの種類
description: '提出物で使用するためにリソースをラップするラッパー。 ラッパーは、割り当てからコピーされた場合、割り当てリソースへのポインターを追加します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 48f4549354603346e39b5e1f6f387b207e2f14ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972483"
---
# <a name="educationsubmissionresource-resource-type"></a>educationSubmissionResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提出物で使用するためにリソースをラップするラッパー。 ラッパーは、割り当てからコピーされた場合、割り当てリソースへのポインターを追加します。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[EducationSubmissionResource を取得する](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |**EducationSubmissionResource**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Delete](../api/educationsubmissionresource-delete.md) | None |**EducationSubmissionResource**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|割り当て Resourceurl|String|このリソースがコピーされた割り当てへのポインター。 この値が null の場合、学生はリソースをアップロードしました。|
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
  "suppressions": []
}
-->
