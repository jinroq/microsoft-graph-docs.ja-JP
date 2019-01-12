---
title: educationAssignmentPointsGrade リソースの種類
description: ポイント グレード タイプに割り当てを設定すると、各提出書類は、このオブジェクトの**submission.grade**プロパティに関連付けられているがあります。 これから educationAssignmentGrade、サブクラスを作成します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d96b84380bc7a6d2298117b5dfeaee25d943efb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982387"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>educationAssignmentPointsGrade リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ポイント グレード タイプに割り当てを設定すると、各提出書類は、このオブジェクトの**submission.grade**プロパティに関連付けられているがあります。 これは、 [educationAssignmentGrade](educationassignmentgrade.md)データが追加されます、ユーザーにこのプロパティをからサブクラスを作成します。 最大のポイントは、 **assignments.grading**プロパティに格納されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|points|単精度浮動小数点型 (Single)|先生をポイント数では、この送信オブジェクト、といいます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
