---
title: educationAssignmentResource リソースの種類
description: 割り当てに関連付けられているリソースを格納するラッパーオブジェクト。 ラッパーは**distributeForStudentWork**プロパティを追加し、このリソースが
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60181a2289b272809cff025abeee83c594ae833e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006431"
---
# <a name="educationassignmentresource-resource-type"></a>educationAssignmentResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

割り当てに関連付けられているリソースを格納するラッパーオブジェクト。 ラッパーは**distributeForStudentWork**プロパティを追加し、このリソースが学生送信にコピーされることを示します。  オブジェクトがコピーされていない場合、各学生には割り当てのリソースへのリンクが表示されます。 学生は、このリソースを更新できません。 これは、教師から、何も有効にしていない学生への配布資料です。 リソースが分散されている場合、各学生は、提出物のリソースリストにこのリソースのコピーを受け取ります。 各学生は、お客様のコピーを変更して、更新のために提出することができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[EducationAssignmentResource を取得する](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |**EducationAssignmentResource**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/educationassignmentresource-update.md) | [educationAssignmentResource](educationassignmentresource.md) |**EducationAssignmentResource**オブジェクトを更新します。 |
|[Delete](../api/educationassignmentresource-delete.md) | None |**EducationAssignmentResource**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|distributeForStudentWork|Boolean|このリソースを各学生送信にコピーして変更および提出する必要があるかどうかを示します。|
|id|String| このリソースの ID。 読み取り専用です。|
|リソース|[educationResource](educationresource.md)|この割り当てに関連付けられているリソースオブジェクト。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
