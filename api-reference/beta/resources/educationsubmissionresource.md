---
title: educationSubmissionResource リソースの種類
description: '提出書類に使用するリソースのラッパーです。 ラッパーは、この課題からコピーされた場合、割り当てリソースにポインターを追加します。  '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 8703072fccb77a2577db6ce0717647e79a47fdc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875986"
---
# <a name="educationsubmissionresource-resource-type"></a>educationSubmissionResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

提出書類に使用するリソースのラッパーです。 ラッパーは、この課題からコピーされた場合、割り当てリソースにポインターを追加します。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[EducationSubmissionResource を取得します。](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |**EducationSubmissionResource**オブジェクトのプロパティと関係を参照してください。|
|[Delete](../api/educationsubmissionresource-delete.md) | なし |**EducationSubmissionResource**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|このリソースのコピー元の割り当てへのポインター。 これが null の場合、受講者は、リソースをアップロードします。|
|id|String| 読み取り専用です。|
|resource|[educationResource](educationresource.md)|リソース オブジェクト。|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
