---
author: daspek
ms.author: dspektor
title: incompleteData リソースの種類
description: IncompleteData ファセットは、リソースが不完全なデータで生成されたことを示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f26317cf16f0773852df35941c00e88df145cc31
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970775"
---
# <a name="incompletedata-resource-type"></a>incompleteData リソースの種類

**Incompletedata**ファセットは、リソースが不完全なデータで生成されたことを示します。
内のプロパティは、データが不完全である理由についての情報を提供する場合があります。

## <a name="properties"></a>プロパティ

| プロパティ                  | 型           | 説明
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | サービスは、指定された時間の前にソースデータを持っていません。
| 制限あり              | Boolean        | アクティビティが多すぎるため、一部のデータが記録されませんでした。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->
