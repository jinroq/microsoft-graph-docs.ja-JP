---
title: educationAssignmentResource リソースの種類
description: 割り当てに関連付けられているリソースを格納するラッパーオブジェクト。 ラッパーは**distributeForStudentWork**プロパティを追加し、このリソースが
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 08a716edabc31c83a7fb3e358fbafd023d5fa784
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334411"
---
# <a name="educationassignmentresource-resource-type"></a>educationAssignmentResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

割り当てに関連付けられているリソースを格納するラッパーオブジェクト。 ラッパーは**distributeForStudentWork**プロパティを追加し、このリソースが学生送信にコピーされることを示します。  オブジェクトがコピーされていない場合、各学生には割り当てのリソースへのリンクが表示されます。 学生は、このリソースを更新できません。 これは、教師から、何も有効にしていない学生への配布資料です。 リソースが分散されている場合、各学生は、提出物のリソースリストにこのリソースのコピーを受け取ります。 各学生は、お客様のコピーを変更して、更新のために提出することができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[educationAssignmentResource を取得する](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |**educationAssignmentResource**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/educationassignmentresource-update.md) | [educationAssignmentResource](educationassignmentresource.md) |**educationAssignmentResource**オブジェクトを更新します。 |
|[削除](../api/educationassignmentresource-delete.md) | なし |**educationAssignmentResource**オブジェクトを削除します。 |

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
