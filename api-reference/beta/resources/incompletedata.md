---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: add1e3612f65e203f2437419cbb105b78025aa0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807512"
---
# <a name="incompletedata-resource-type"></a>incompleteData リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**IncompleteData**ファセットは、不完全なデータとリソースが生成されたことを示します。
内でプロパティがについての情報を提供するには、不完全なデータがある理由です。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a>プロパティ

| プロパティ                  | 種類           | 説明
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | サービスには、指定された時間の前にソース データがありません。
| wasThrottled              | ブール型        | データの一部は、過剰な活動のため録画されませんでした。

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
