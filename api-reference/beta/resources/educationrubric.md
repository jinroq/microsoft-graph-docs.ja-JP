---
title: educationRubric リソースの種類
description: 割り当てに関連付けることができる適用
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b43b611465af4dabb62d9dd741eb9a8670f241b9
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173238"
---
# <a name="educationrubric-resource-type"></a>educationRubric リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

割り当てに関連付けることができる、その他の方法。 **EducationUser** (教師) に関連付けられており、1つ以上の**educationAssignment**リソースに添付されます。 

詳細については、「[教育機関](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview)向けの概要」を参照してください。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [EducationRubric を取得する](../api/educationrubric-get.md) | [educationRubric](educationrubric.md) | EducationRubric オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [EducationRubric の更新](../api/educationrubric-update.md) | [educationRubric](educationrubric.md) | EducationRubric オブジェクトを更新します。 |
| [EducationRubric の削除](../api/educationrubric-delete.md) | None | EducationRubric オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|createdBy|[identitySet](identityset.md)|このリソースを作成したユーザー。|
|createdDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|description|[itemBody](itembody.md)|このテンプレートの説明。|
|displayName|String|この名前を指定します。|
|変化|[educationAssignmentGradeType](educationassignmentgradetype.md)|この EducationAssignmentPointsGradeType の値の種類。非ポイントを指定しない場合は null、ポイント単位の場合は[](educationassignmentpointsgradetype.md)になります。|
|lastModifiedBy|[identitySet](identityset.md)|リソースを最後に変更したユーザー。|
|lastModifiedDateTime|DateTimeOffset|リソースが最後に変更された時点の時刻。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|高度|[プリンシパル](rubriclevel.md)コレクション|このテンプレートを構成するレベルのコレクション。|
|満たし|の[最高品質](rubricquality.md)のコレクション|このテンプレートを構成する品質のコレクション。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [{"@odata.type": "microsoft.graph.rubricLevel"}],
  "qualities": [{"@odata.type": "microsoft.graph.rubricQuality"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubric resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->