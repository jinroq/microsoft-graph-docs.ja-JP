---
title: educationSubmissionResource リソースの種類
description: '提出書類に使用するリソースのラッパーです。 ラッパーは、この課題からコピーされた場合、割り当てリソースにポインターを追加します。  '
ms.openlocfilehash: 243d0d8683683df19f7787f7cf6298770950455f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072588"
---
# <a name="educationsubmissionresource-resource-type"></a>educationSubmissionResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

提出書類に使用するリソースのラッパーです。 ラッパーは、この課題からコピーされた場合、割り当てリソースにポインターを追加します。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[EducationSubmissionResource を取得します。](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |**EducationSubmissionResource**オブジェクトのプロパティと関係を参照してください。|
|[削除](../api/educationsubmissionresource-delete.md) | なし |**EducationSubmissionResource**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|このリソースのコピー元の割り当てへのポインター。 これが null の場合、受講者は、リソースをアップロードします。|
|id|String| 読み取り専用。|
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