---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: incompletedata
localization_priority: Normal
ms.openlocfilehash: 40c1b782384076eefc986f67dc1736f191feb7b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339967"
---
# <a name="incompletedata-resource-type"></a>incompletedata リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**incompletedata**ファセットは、リソースが不完全なデータで生成されたことを示します。
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
