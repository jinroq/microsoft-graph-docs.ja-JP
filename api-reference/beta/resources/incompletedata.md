---
author: daspek
description: IncompleteData ファセットは、リソースが不完全なデータで生成されたことを示します。
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 23d78fa3605259031fc2c408e93a0461bb12cb28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006284"
---
# <a name="incompletedata-resource-type"></a>incompleteData リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Incompletedata**ファセットは、リソースが不完全なデータで生成されたことを示します。
内のプロパティは、データが不完全である理由についての情報を提供する場合があります。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a>プロパティ

| プロパティ                  | 型           | 説明
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | サービスは、指定された時間の前にソースデータを持っていません。
| 制限あり              | Boolean        | アクティビティが多すぎるため、一部のデータが記録されませんでした。

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
