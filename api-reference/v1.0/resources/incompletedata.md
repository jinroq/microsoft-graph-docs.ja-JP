---
author: daspek
ms.author: dspektor
title: incompleteData リソースの種類
description: IncompleteData ファセットは、リソースが不完全なデータで生成されたことを示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0ac77c5dc4daed9330c4fb71185e9505feee5048
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029240"
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
