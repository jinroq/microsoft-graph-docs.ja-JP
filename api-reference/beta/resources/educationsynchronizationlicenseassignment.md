---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザー アカウントに割り当てるにはライセンス情報を表します。 新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。
author: mmast-msft
ms.openlocfilehash: 478d939c8f4c6a0bc1971d66afc4ecc7ae640e39
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344395"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>educationSynchronizationLicenseAssignment リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザー アカウントに割り当てるにはライセンス情報を表します。 新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。

## <a name="properties"></a>Properties

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **appliesTo** | string | ライセンスを割り当てるにはユーザーのロールの種類です。 使用可能な値は、`student`、`teacher` です。         |
| **skuIds** | 文字列のコレクション |  割り当てるライセンスの SKU 識別子を表します。        |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
