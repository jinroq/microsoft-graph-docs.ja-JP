---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザーアカウントに割り当てるライセンス情報を表します。 リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5d1aaf2784434525e2fa750ad78966d6cbf15bc8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750137"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>educationSynchronizationLicenseAssignment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーアカウントに割り当てるライセンス情報を表します。 リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **appliesTo** | string | ライセンスに割り当てるユーザーの役割の種類。 可能な値は、`student`、`teacher`、`faculty` です。         |
| **skuIds** | 文字列のコレクション |  割り当てるライセンスの SKU 識別子を表します。        |

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
