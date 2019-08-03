---
title: educationFeedbackOutcome リソースの種類
description: テキスト形式でフィードバックを提供する educationOutcome。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e61538a62a1bb267b0a13b98b17e9b69a8ceed92
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173252"
---
# <a name="educationfeedbackoutcome-resource-type"></a>educationFeedbackOutcome リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テキスト形式の[educationOutcome](educationoutcome.md)オブジェクトに対するフィードバックを表します。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [EducationOutcome の更新](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | EducationOutcome オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|feedback|[educationFeedback](educationfeedback.md)|教師が生徒に書面でフィードバックを送信します。|
|publishedFeedback|[educationFeedback](educationfeedback.md)|成績が生徒にリリースされたときに行われるフィードバックプロパティのコピー。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "publishedFeedback": {"@odata.type": "microsoft.graph.educationFeedback"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->