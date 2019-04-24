---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザーアカウントに割り当てるライセンス情報を表します。 リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507099"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>educationSynchronizationLicenseAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーアカウントに割り当てるライセンス情報を表します。 リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **appliesTo** | string | ライセンスに割り当てるユーザーの役割の種類。 可能な値は、`student`、`teacher` です。         |
| **skuids** | 文字列のコレクション |  割り当てるライセンスの SKU 識別子を表します。        |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationlicenseassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
