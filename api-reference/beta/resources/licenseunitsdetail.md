---
title: licenseUnitsDetail リソースの種類
description: subscribedSku エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。
localization_priority: Normal
ms.openlocfilehash: d6fb464eaf9c1247d21ad9effb2b70c6bdaa1c3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883511"
---
# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[subscribedSku](subscribedsku.md) エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:-------------|:-----|:----------|
|enabled|Int32| 有効になっている単位の数です。 |
|suspended|Int32| 利用停止中の単位の数です。 |
|warning|Int32| 警告ステータスのユニットの数です。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
